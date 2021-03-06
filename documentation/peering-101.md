Peering 101
===========

Once you've received your brand new, shiny Meshbox, you need "peers" to connect to Hyperboria. Your router will come preconfigured with preset peers, but these will expire approximately 6 months after the shipping date.

These are usually found by asking on [IRC](https://wiki.projectmeshnet.org/IRC). Please note that just asking for a peer will not guarantee you'll get a peer! Most people will peer with you if you introduce yourself, and tell them what some of your interests are and what you'd like to contribute. It's also heavily recommended to look and see if there is a localMesh near you, as they will usually provide closer peering to you.

When your peers send you the connection details, connect to your router's web interface, usually located at [OpenWRT.lan](http://openwrt.lan) if you are connected through one of the router's LAN ports or by WiFi.

After you're connected, log in with the password you set when you first set up the router. If you haven't done that, set a password. Next, browse to Services -> cjdns. Here an overview of cjdns and its connections are shown, and should look similar to the picture below.

![UI screenshot](https://raw.githubusercontent.com/SeattleMeshnet/meshbox/ee9340a6421fe0342eda44b23028143923bb65ee/screenshot.png)


Next, go to peers, and enter in the IP, password and public key in the corresponding boxes under Outgoing UDP Peers..

Next, reboot the router by going to System -> Reboot, and follow the instructions to reboot the router.

You're all set!
