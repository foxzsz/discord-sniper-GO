# discord-sniper-GO
![image](https://user-images.githubusercontent.com/82937328/164210653-bc018e3b-d2f7-4a6d-b013-623c29c4f58d.png)

**discord-sniper-GO** is a very-fast and efficient mulithreaded tool used to snipe discord vanities with ease. 

**NOTE: As I haven't fully tested this with high-tier vanities, it is recommended to first test it on a free/claimable vanity before attempting to swap anything high-tier to ensure that the account  is able to claim. If you use this tool to swap / autoclaim high-tier vanitys please do let me know what your experience with this tool is on telegram: @uceicViwpvBo**

## **Features** :
- Automatically send notifications to webhook
- Supports sniping a lot of vanities simultaneously
- Advanced proxy switching mechanism
- Multiple modes used to claim the vanities (fasthttp and sockets)


## Basic Usage
1) Building the program by source
2) Configure your "config.yml" file ( webhook, guildid, amplify and token)
3) Add your proxies to the "proxies.txt" file
4) Add your vanity list to the "vanities.txt" file
5) Run the binary and wait for the program to snipe


## How to build from source
1) First download the suitable golang version from the following link: https://go.dev/dl/
2) Clone / download the code from this github repository
3) Either cd to the directory where the code is or open a terminal in the directory
4) Type go build .
5) Then you should have a executable which you can then use too snipe


## Configuration

| Name | Description | 
| ---  | ---  |
| `amplify` | Amount of goroutines per vanity, if there are 5 vanities and amplify is 6 it means there will be 6 goroutines per vanity
| `token` | Discord token which has access to changing the vanity of server
| `webhook` | Webhook for sending notifications
| `guildid` | Guildid of server which has access to the vanity feature
| `usesockets` | It is recommended to leave this option disabled unless you know how the code works, as it is currently experimental
| `socketchannels` | Amount of socket channels, ignore this if you are not using the usesockets option
