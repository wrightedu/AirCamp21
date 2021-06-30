for starters:
`nmap 10.0.0.25` gives the following

```
Starting Nmap 7.60 ( https://nmap.org ) at 2021-06-30 16:37 UTC
Nmap scan report for 10.0.0.25
Host is up (0.0057s latency).
Not shown: 996 closed ports
PORT      STATE SERVICE
22/tcp    open  ssh
80/tcp    open  http
9999/tcp  open  abyss
10000/tcp open  snet-sensor-mgmt

Nmap done: 1 IP address (1 host up) scanned in 0.12 seconds
```

But we know there are 7 flags in this challenge.  There are two main challenges:

* find the other 3 ports that are open (hint: `nmap`)
* find out how to get a flag off of each port (a good start is `nc` but 22 and 80 are going to need something special relating to what normally runs on these ports)
