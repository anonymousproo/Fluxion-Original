# Fluxion-Original

<p align="center"><img src="https://github.com/anonymousproo/Fluxion-Original/blob/main/logos/trtrrrr.png?raw=true" /></p>
<p align="center"><img src="https://github.com/anonymousproo/Fluxion-Original/blob/main/logos/444.jpg?raw=true" /></p>

# Fluxion is the future of MITM WPA attacks
Fluxion is a remake of linset by vk496 with (hopefully) less bugs and more functionality. It's compatible with the latest release of Kali (rolling). The attack is mostly manual, but experimental versions will automatically handle most functionality from the stable releases.

## :trident: FAQ

#### "Clients are not automatically connected to the fake access point"
This is a social engineering attack and it's pointless to drag clients in automatically. The script relies on the fact that a user should be present in order to enter the wireless credentials.

#### "There's no Internet connectivity in the fake access point"
There shouldn't be one. All of the traffic is being sinkholed to the built in captive portal via a fake DNS responder in order to capture the credentials.

#### "Fake sites don't work"
There might be a problem with lighttpd. The experimental version is tested on lighttpd 1.439-1, anything neweer may break functionality. If you have problems, please use the stable version.

#### "Experimental menu is not responsive"
In the experimental version it will automatically check the handshake. I will fix the menu shortly. If you need a GUI, use the stable version (which doesn't automatically control handshakes).

#### "I need to sign in (on Android)"
This is how the script works. The fake captive portal is set up by the script itself to collect the credentials. Don't freak, it's al okay.

#### "The MAC address of the fake access point differs from the original"
The MAC address of the fake access point differs by one octet from the original in order to prevent fluxion deauthenticating clients from itself during the session. 

## Installation

before you do the following steps.

Download  clone. https://github.com/anonymousproo/fluxion

## Switch to tool's directory

cd fluxion 

## Run fluxion

chmod +x fluxion.sh

./fluxion.sh

## missing dependencies will be manually installed (install big problem is pyrit)

## how to install pyrit missing file 

watch before you do the following steps

click here https://bit.ly/3b3hLb1

## how to solve fluxion tool pyrit missing kali linux 2020 

click here https://bit.ly/3b3hLb1


## Our Best Hacking & Security Guides........

what's app: https://bit.ly/2V1zwSt

## Updates
If you want to submit a feature, do so by labeling your issue as an "enhancement" or submit a PR. I don't have enough time to make daily changes to fluxion, sorry.
we are fluxion tool handshake solved the problem

## :white_check_mark: Included dependency versions
1. Aircrack : 1:1.2-0~rc4-0parrot0
2. Lighttpd : 1.439-1
3. Hostapd  : 1:2.3-2.3 _If you want to compare this type `dpkg -l | grep "name"`_

## :scroll: Changelog
Fluxion gets weekly updates with new features, improvements and bugfixes.
Be sure to check out the [changelog here](https://github.com/FluxionNetwork/fluxion/commits/master).

## :octocat: How to contribute
All contributions are welcome! Code, documentation, graphics or even design suggestions are welcome; use GitHub to its fullest. Submit pull requests, contribute tutorials or other wiki content -- whatever you have to offer, it would be appreciated!

## :book: How it works
* Scan the networks.
* Capture a handshake (can't be used without a valid handshake, it's necessary to verify the password)
* Use WEB Interface *
* Launch a FakeAP instance to imitate the original access point
* Spawns a MDK3 process, which deauthenticates all users connected to the target network, so they can be lured to connect to the FakeAP and enter the WPA password.
* A fake DNS server is launched in order to capture all DNS requests and redirect them to the host running the script
* A captive portal is launched in order to serve a page, which prompts the user to enter their WPA password
* Each submitted password is verified by the handshake captured earlier
* The attack will automatically terminate, as soon as a correct password is submitted

## :heavy_exclamation_mark: Requirements

A Linux-based operating system. We recommend Kali Linux 2019.4. Without external wifi card is recommended.
Just need internal wifi card is recommended.

## :octocat: Credits
1. l3op - contributor
2. dlinkproto - contributor
3. vk496 - developer of linset
4. Derv82 - @Wifite/2
5. Princeofguilty - @webpages
6. Photos for wiki @http://www.kalitutorials.net
7. Ons Ali @wallpaper
8. PappleTec @sites

## Disclaimer

***Fluxion is intended to be used for legal security purposes only, and you should only use it to protect networks/hosts you own or have permission to test. Any other use is not the responsibility of the developer(s).  Be sure that you understand and are complying with the Fluxion licenses and laws in your area.  In other words, don't be stupid, don't be an asshole, and use this tool responsibly and legally.***
