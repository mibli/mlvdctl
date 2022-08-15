# Mullvad Control (mlvdctl)

Simple minimal dependency tool to help You easily manage Mullvad VPN connection using systemctl
WireGuard-quick services, from the terminal.

Uses sudo privileges, so make sure to check the source.

![preview generated with asciicast and svg-term-cli](doc/preview.svg)

## Requirements

* wg-quick
* Mullvad wireguard configurations in `/etc/wireguard` directory!

## Example usage:

    mlvdctl             # interactive
    mlvdctl -r          # select random country and server
    mlvdctl -c ro -s 4  # select server 4 in Romania
    mlvdctl -d          # stop vpn connection
    mlvdctl -e          # start vpn connection
    mlvdctl -l          # show status of vpn connection
