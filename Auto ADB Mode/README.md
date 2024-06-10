# Auto ADB over TCPIP
A flow to automatically activate wireless debugging and set ADB over TCP/IP port 5555, allowing you to continue using your device seamlessly without manual reconfiguration after every restart.

**Table of Contents**
1. [Getting Started](#getting-started)
	- [Download](#download)
	- [Configuration](#configuration)
2. [Blocks](#blocks)
	- [Broadcast Receive](#broadcast-receive)
	- [System Setting Set](#system-setting-set)
	- [Network Service Discover](#network-service-discover)
	- [ADB Protocol Set](#adb-protocol-set)
3. [How Does It Work?](#how-does-it-work)
4. [Troubleshooting](#troubleshooting)
5. [Contribute](#contribute)
---
# Getting Started
## Download
1. Open Automate and go to community.
2. Find [Auto ADB over TCPIP](https://llamalab.com/automate/community/flows/48004) in community tab.
3. Click on Download and go to flows tab.

## Configuration
1. Open Automate settings
	1. Find **Privileges** under **Access Control**, tap then give access to:
		- `Access location in the background`
		- `Show Notifications`
		- `Modify System Settings`
		- `Ignore App Hibernation`
		- `Ignore Battery Optimizations`
		- `Schedule Exact Alarms`
	2. Find **Privileged service start method** under **Privileged & Superuser**
		- Select `Android Debug Bridge (ADB)`
		- Go to **Developer options** and turn on **Wireless debugging**:
			- Check `Always allow on this network`.
			- Select allow on `allow wireless debugging on this network`.
		- Tap on **Pair Device with pairing code**.
			- Enter `Wi-Fi pairing code` to `Enter code that's shown` dialog at the top.
	3. Check **Run on system startup** under **Safety**.
2. Go to the Flows tab and start the flow.
> [!Note]
> - Problem? Refer to [Troubleshooting](#troubleshooting).
> - Didn't find the fix for your issue? Ask the question in the comments **in detail**.
---
# Blocks
## [Broadcast Receive](https://llamalab.com/automate/doc/block/broadcast_receive.html)

|     Action     |
| :------------: |
| Boot Completed |
## [System Setting Set](https://llamalab.com/automate/doc/block/system_setting_set.html)

| Category |        Name        | Value |
| :------: | :----------------: | :---: |
|  Global  | "adb_wifi_enabled" |  `1`  |
## [Network Service Discover](https://llamalab.com/automate/doc/block/nsd_discover.html)

|      Service Type       |
| :---------------------: |
| "_adb-tls-connect._tcp" |
## [ADB Protocol Set](https://llamalab.com/automate/doc/block/adb_protocol_set.html)

| Protocol | TCP/IP Port | Hostname | Port  |
| :------: | :---------: | :------: | :---: |
|  TCP/IP  |    5555     |  hosts   | ports |
> [!Note]
> - Hostname and Port are using variable we got from Network Service Discover.
---
# How Does It Work?

1. **Boot Completion Wait:**
    - The flow waits until the device finishes booting using [Broadcast Receive](#broadcast-receive) block.
2. **ADB Restart Notification:**
    - After boot completion, it displays a notification asking if the user wants to restart ADB in TCPIP mode.
3. **Wi-Fi Connection Check:**
    - If the user clicks on the notification, it immediately checks if the device is connected to Wi-Fi.
    - If connected, it proceeds; otherwise, it waits for the device to connect to Wi-Fi.
4. **Enable Wireless Debugging:**
    - It enables wireless debugging using the [System Setting Set](#system-setting-set) block.
5. **Hostname and Port Discovery:**
    - The flow attempts to find the hostname and port for connection using the [Network Service Discover](#network-service-discover) block.
    - If no information is found, it continues trying until it discovers the hostname and port.
6. **Set TCPIP to 5555:**
    - It sets the TCPIP to port 5555 using the [ADB Protocol Set](#adb-protocol-set) block.
    - If this step fails, the flow turns off wireless debugging and starts again from block 4.

> [!Note]
> - For first-time use, the flow starts from the **Is Wi-Fi Connected** block to ensure everything is working as expected.
---
# Troubleshooting

- `com.llamalab.automate.RequiredArgumentNullException: alias`
	- Install Generated Key, then add it to Keychain alias.

- `android.security.KeyChainException: Certificate or private key inaccessible:{certificate}`
	- Re-install Generated Key, then add it to Keychain alias.

- `android.system.ErrnoException: isConnected failed: ECONNREFUSED (Connection refused)`
	- Try _Forget privileged service ADB keys_, then pair again.
- `javax.net.ssl.SSLProtocolException: Read error: ssl=0xb400007dbbf10988: Failure in SSL library, usually a protocol error`
	- Try pairing again. 
- `error:10000416:SSL routines:OPENSSL_internal:SSLV3_ALERT_CERTIFICATE_UNKNOWN (external/boringssl/src/ssl/tls_record.cc:592 0xb400007dbaa83600:0x00000003)`
	- Try pairing again. 
# Contribute
If you find any mistakes in the flow or missing information on this documentation or want to support financially, you can do so in the comments by commenting.

Thank you for using the flow.