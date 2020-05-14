Script for adding userguard users

Creates folders and files for configuring new users.

Default folder is /etc/wireguard

Folder /etc/wireguard/keys is for keys - this folder should exist and contain server keys (private and public).

Folder /etc/wireguard/userconf is for user configs (you can send them to users for import).

File /etc/wireguard/lastip uses for setting newuser ip.

File /etc/wireguard/wg0.conf - WireGuard daemon config

usage: ./useradd -u username

After adding new user script restarts wireguard daemon wg-quick@wg0.
