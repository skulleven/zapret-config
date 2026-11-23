# Introduction
This repo holds all of the zapret configs that I use day to day. Compiled as a result of over 5 hours of testing by hand. Putting them here incase people can use these instead of staring at a terminal screen for hours.

# Overview of the configs

skulleven - The config I've made mainly for Discord access.
kutuphane - The config I've made to bypass the restrictions on the library Wi-Fi

# Explaining "kutuphane"

The library Wi-Fi uses a pretty common FortiGate setup. Luckily it only checks if the domain name is included in the list of blocked websites in plain text. So bypassing it just required some zapret magic. 

Used nfqws instead of a SOCKS5 approach with tpws cause Steam got really upset when I used a SOCKS5 proxy to connect to the client. Also it allows for us to make a cleaner implementation.

The rest of the rules are gotten from blockcheck.sh and GoodbyeDPI rules since that seems to bypass it on Windows.