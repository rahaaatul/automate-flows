# Introduction

Easily turn on/off Private DNS or change the hostname.

Table of contents:
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
    - [How to edit DNS' in **Private DNS Changer** flow?](#how-to-edit-dns-in-private-dns-changer-flow)
    - [How to add more DNS' in **Private DNS Changer** flow?](#how-to-add-more-dns-in-private-dns-changer-flow)
- [Roadmap](#roadmap)

# Private DNS

Turns on/off private DNS with a tap of a QS Tile.

## Features
- Tap QS tile to turn on or off Private DNS.
- Tap and hold QS tile to open Private DNS settings. 

## Requirements

1. Permissions:
   - Appear on top of other apps or parts of the screen
   - Modify System Settings
   - Ignore Battery Optimizations

## Installation

1. Download [Private DNS](https://llamalab.com/automate/community/flows/48325) from Automate community.
2. Add one empty automate QS Tiles.
3. Start flow.

---

# Private DNS Changer

Changes Private DNS hostname. It has 2 options to choose from:

1. Change DNS to one or more defined hostnames with a tap of a QS Tile.
2. Open a list of DNS' to choose from with a tap of a QS Tile.

> [!Caution]
> - `Tap QS tile to change DNS` flow supports only two DNS'.
> - Do not add more than two.

> [!Important]
> - You can add unlimited DNS' in `Tap QS tile to show DNS List`.

> [!Note]
> - Thinking of a way to cycle through multiple DNS, tapping only one QS tile multiple times.

## Features
- Tap QS tile to change Private DNS.
- Tap QS tile to open a list of DNS to choose from.

## Requirements

1. Permissions
    - Modify System Settings
    - Ignore Battery Optimizations

## Installation

1. Download [Private DNS Changer](https://llamalab.com/automate/community/flows/48328) from Automate community.
2. Add one or two empty automate QS Tiles.
3. Start flow/s.

---

# Frequently Asked Questions

## Private DNS 
⚒️ Content **Under Construction**

## Private DNS Changer

### How to edit DNS' in **Private DNS Changer** flow?

   1. Open and edit **Private DNS** flow.
   2. Tap on `Set variable dnsOptions`.
   3. In `Input arguments` field you'll find:

        ```sh
        concat("dns.adguard-dns.com", "dns.google")
        ```

   4. Replace the DNS' you want to change inside double quotes.
   5. Save and start flow.


### How to add more DNS' in **Private DNS Changer** flow?

   1. Open and edit **Private DNS Changer** flow.
   2. Tap on `Set variable dnsOptions` in `Tap QS tile to show DNS List` flow.
   3. In `Input arguments` field you'll find:

        ```sh
        concat("dns.adguard-dns.com", "dns.google", "one.one.one.one")
        ```

   4. Add a `,` comma at the end before the closing parenthesis and add another DNS in `""` double quotes.
   5. Save and start flow.

# Roadmap
- Merge two flows together.
- Tap to cycle through DNS list.
- Tap and hold to show the DNS list to choose DNS from.