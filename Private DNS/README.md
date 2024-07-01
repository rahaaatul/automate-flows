# Private DNS Flows

## Introduction

Easily turn on/off Private DNS or change the DNS Host.

Table of contents:

- [Private DNS Flows](#private-dns-flows)
  - [Introduction](#introduction)
  - [Private DNS](#private-dns)
    - [Features](#features)
    - [Requirements](#requirements)
    - [Installation](#installation)
  - [Private DNS Changer](#private-dns-changer)
    - [Features](#features-1)
    - [Requirements](#requirements-1)
    - [Installation](#installation-1)
  - [Frequently Asked Questions](#frequently-asked-questions)
    - [Private DNS](#private-dns-1)
    - [Private DNS Changer](#private-dns-changer-1)
      - [How to add more DNS' in **Private DNS Changer** flow?](#how-to-add-more-dns-in-private-dns-changer-flow)

## Private DNS

> ***Tap QS Tile to turn on/off your Private DNS.***

### Features

- Tap QS tile to turn on or off Private DNS.
- Tap and hold QS tile to open Private DNS settings.

### Requirements

- Android 9 or later.
- Permissions:
  - Appear on top of other apps or parts of the screen.
  - Modify System Settings.
  - Ignore Battery Optimizations.
- Empty Tile added in Quick Switcher.

### Installation

1. Download [Private DNS](https://llamalab.com/automate/community/flows/48325) from Automate community.
2. Add one empty Automate QS Tiles.
3. Start flow.

## Private DNS Changer

Changes Private DNS hostname. It has 2 options:

- Tap QS Tile to change DNS' chronologically.
- Long press QS Tile to get a list of DNS' to set.

### Features

- Tap QS tile to change Private DNS.
- Tap QS tile to open a list of DNS to choose from.

### Requirements

- Android 9 or later.
- Permissions:
  - Modify System Settings.
  - Ignore Battery Optimizations.
- Empty Tile added in Quick Switcher.

### Installation

1. Download [Private DNS Changer](https://llamalab.com/automate/community/flows/48328) from Automate community.
2. Add one empty Automate QS Tile.
3. Start flow.

---

## Frequently Asked Questions

### Private DNS

⚒️ Content **Under Construction**

### Private DNS Changer

#### How to add more DNS' in **Private DNS Changer** flow?

   1. Open and edit **Private DNS Changer** flow.
   2. Tap on `Set variable dnsList`.
   3. In `Input arguments` field you'll find:

        ```sh
        ["dns.adguard-dns.com", "dns.google", "one.one.one.one"]
        ```

   4. Add a `,` comma at the end before the closing parenthesis and add another DNS in `""` double quotes. Like this:

        ```sh
        ["dns.adguard-dns.com", "dns.google", "one.one.one.one", "dns11.quad9.net"]
        ```

   5. Save and start the flow.
