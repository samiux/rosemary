# Rosemary 迷迭香 - Intrusion Detection and Prevention System  防御入侵系统

Networks and computers that are opened to the public facing hacker attacks from all over the world every day.  Once we are compromised, we would be one of the cyber crime victims.  Our Rosemary is a high performance and ultra-low latency Intrusion Detection and Prevention System (IDPS).  Unlike well known and famous brands for large business enterprises in the market,  Rosemary is available free of charge that everyone can afford.  It is ideal for home and Small Office Home Office (SOHO). 

Not a Network Security Monitoring (NSM) or Information Security (InfoSec) expert?  No problem!  Our Rosemary really is the "Plug, Play and Forget" system of your dreams, it is totally transparent.  Don't be the next cyber crime victims, try Rosemary now!

Rosemary is designed by a hacker to defend against hackers. He knows what hackers are doing and thinking, regardless of whether they are ethical or malicious.

## FEATURES

- Blocks known malicious activities  
- Compatible with Bittorrent and 4K video streaming  
- Ultra-low latency for demanding online games  
- Compatible with Microsoft Windows, GNU Linux, Apple macOS, Apple iOS, Google Android and Huawei HarmonyOS  
- No subscription fee  
- Automatically update  
- Plug, Play and Forget!  
- Totally transparent  
- Setup is not required   

## HARDWARE

### NanoPI R6S

- 8 cores CPU  
- 8GB RAM  
- 32GB storge  
- 3 network interfaces (2 x 2.5Gbps, 1 x 1Gbps)   
- Max. power consumption 5W, fanless, no noise  
- Max. WAN traffic flow up to 2.5Gbps  
- Slightly larger than a credit card  
- 96.5mm (L) x 68mm (W) x 30mm (H)   

### NanoPi R5S (Not Recommended)

- 4 cores CPU  
- 4GB RAM  
- 16GB storge  
- 3 network interfaces  (2 x 2.5Gbps, 1 x 1Gbps)    
- Max. power consumption 5W, fanless, no noise  
- Max. WAN traffic flow up to 2.5Gbps  
- Slightly larger than a credit card  
- 94.5mm (L) x 68mm (W) x 30mm (H)  

## INSTALLATION

A 16GB SD Card (at least Class 10) is required for the installation.  

Download the [SD Card image (467MB)](https://drive.google.com/file/d/17DbJ0On05b1-672aO-Zq1PLGT5ljAP4F/view?usp=sharing) at Google Drive.

Download [Balena Etcher](https://www.balena.io/etcher) at its official site and burn to the SD Card.

### Checksum

sha256 d757b5a84571d6fb8862f3496e3923988e104be2b38ca14891fcad9002846081  rk3588-sd-rosemary-5.10-arm64-20230304.zip  
sha256 a7e9d911a9298e677cbfd0dffbfa4a497f4f346056374ef4d0a765ab5aab5fe1  rk3588-sd-rosemary-5.10-arm64-20230304.img  

## DEPLOYMENT  

The following is the recommended connection method of Rosemary.  However, you can connect it behind router too.

```bash
            (WAN)             (LAN1 to Router's WAN)          (Router's LAN)          
   Modem ----------- Rosemary ----------------------- Router ----------------- PCs & Laptops
                          |                           (WIFI)                      
                          |                             | (Router's LAN)                   
                          +-----------------------------+
                              (LAN2 to Router's LAN)
```
```bash
                                                                                +------- Laptops
                                                                                |
            (WAN)           (LAN1 to Router's WAN)     (Switch's LAN)           |
   Modem ----------- Rosemary ------------------ Router -------- Switch --------+
                          |                      (WIFI)             |           |
                          |                                         |           |
                          +-----------------------------------------+           +------- PCs
                                   (LAN2 to Switch's LAN)

```
```bash
                                                                    +------- WIFI AP
                                                                    |
            (WAN)          (LAN1 to Switch Port #1)                 |
5G Modem ----------- Rosemary ------------------ Switch ------------+
WIFI Router (unused)      |                        |                |
                          |                        |                |
                          +------------------------+                +------- PCs & Laptops
                                    (LAN2)

```

Do NOT use the wifi that comes with 5G modem as the traffic flow will NOT be protected by Rosemary.

## FAQ  

### When will the rules are updated?

#### 24/7
Between 0600 and 0630 hours every day, Rosemary will do the housekeeping and updating.  The defending work of Rosemary may be interrupted during this period.  

#### non 24/7
Rosemary can be turned off and it is not required to operate 24/7.  The update will be carried out within half an hour when the Rosemary is booting up.  It is advised NOT to turn off the Rosemary between 0600 and 0630 hours as it will do the update automatically.  If you do so, you may break the Rosemary.  Meanwhile, if you turn off the Rosemary within half an hour of the booting up, you may also break the system too.    

### How many detecting / blocking rules in Rosemary?  
There are over 40,000 rules in Rosemary and they are all free of charge.  The number of rules are increasing.    

### Do you recommend to access Rosemary via SSH in internet?
For security purpose, it is NOT recommended to connect Rosemary via SSH in internet.  However, you may connect Rosemary via SSH in intranet.  The username and password are "rosemary".    

### Can Rosemary decrypt the SSL/TLS traffic?
Rosemary cannot decrypt the SSL/TLS traffic well.  However, it can handle a limited SSL/TLS traffic flow.  Therefore, it is not ideal for using it as Web Application Firewall (WAF).  For example, Rosemary can detect and drop self signed SSL/TLS certificate traffic and etc.  

### Do I also need anti-virus?
Yes, anti-virus is required.  You are also advised to install the following add-ons or extensions for your browser such as Firefox or Chrome in order to increase the security for surfing the internet.

- uBlock Origin  
- Ghostery  
- Malwarebytes Browser Guard  
- Avast Online Security & Privacy  
- MalwareAI Browser Security  
- VT4Browsers  

## YOUTUBE REVIEW

- [NanoPi R6S - Unboxing and Quick Overview](https://www.youtube.com/watch?v=-rlJ_80d01U)  
- [NanoPi R6S Linux Review - Rockchip RK3588S with dual 2.5GbE + 1GbE](https://www.youtube.com/watch?v=gCBNWGhp8gM)  
- [NanoPi R6S - Wireguard & OpenVPN Throughput Test](https://www.youtube.com/watch?v=YC16CsEYN6g)  
- [NanoPi R6S - 2.35Gbps Throughput with only 5W of Power Consumption](https://www.youtube.com/watch?v=UMbTibi3n2k)  
- [NanoPi R6S Bootup - Firmware Update (eMMC) - PPPoE Speedtest](https://www.youtube.com/watch?v=WylvVwlDrFg)  
