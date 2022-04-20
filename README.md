# dns-spoof
Python script that allows you to spoof the dns requests

`You will have to launch MITM attack before you perform dns spoofing.`

<a href='https://github.com/itzVort3x1/arp-spoof'>Click here For the code to launch MITM Attack</a>

NOTE:
<br />
1) If you want to test it on the same system run the following two commands:
   1) ```iptables -I INPUT -j NFQUEUE --queue-num 0```
   2) ```iptable -I INPUT -j NFQUEUE --queue-num 0```
   <br/>
   <p>This will help you create a queue in the iptables which will be later accessed by the python program.</p>
2) If you want to test it against another system in the same network
   1) ```iptables -I FORWARD -j NFQUEUE --queue-num 0```
