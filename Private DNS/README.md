# Introduction

Easily turn on/off Private DNS or change the hostname.

Table of contents:
- [Introduction](#introduction)
  - [Private DNS](#private-dns)
  - [Private DNS Changer](#private-dns-changer)
    - [Requirements](#requirements)
    - [Installation](#installation)
- [Frequently Asked Questions](#frequently-asked-questions)

## Private DNS

⚒️ Content **Under Construction**
<!Turns on/off private DNS with a tap of a QS Tile.>

<!Download [Private DNS](https://llamalab.com/automate/community/flows/48325) from Automate community.>

## Private DNS Changer

Changes Private DNS hostname. It has 2 options to choose from:
  1. Changes DNS to one or more defined hostnames with a tap of a QS Tile.
  2. Opens a list of DNS' to choose from with a tap of a QS Tile.

> [!Caution]
> - `Tap QS tile to change DNS` flow supports only two DNS'.
> - Do not add more than two.

> [!Important]
> - You can add unlimited DNS' in `Tap QS tile to show DNS List`.

> [!Note]
> - Thinking of a way to cycle through multiple DNS, tapping only one QS tile multiple times.


### Requirements

1. Permissions
    1. Modify System Settings
    2. Ignore Battery Optimizations

### Installation

1. Download [Private DNS Changer](https://llamalab.com/automate/community/flows/48328) from community.
2. Add empty automate QS Tiles.
3. Start flow/s.

# Frequently Asked Questions

* How to edit DNS in **Private DNS** flow?

    1. Open and edit **Private DNS** flow.
    2. Tap on `Set variable dnsOptions`.
    3. In `Input arguments` field you'll find:

        ```sh
        concat("dns.adguard-dns.com", "dns.google")
        ```

    5. Replace the DNS' you want to change inside double quotes.
    6. Save and start flow.


* How to add more DNS in **Private DNS Changer** flow?
  1. Open and edit **Private DNS Changer** flow.
  2. Tap on `Set variable dnsOptions`.
  3. In `Input arguments` field you'll find:

        ```sh
        concat("dns.adguard-dns.com", "dns.google", "one.one.one.one")
        ```

  4. Add a `,` comma at the end before the closing parenthesis and add another DNS in `""` double quotes.
  5. Save and start flow.
