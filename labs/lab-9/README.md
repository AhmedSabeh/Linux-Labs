# Lab 9: Network Exploration

## Objective
Practice testing network connectivity, checking network interfaces, and downloading web content.

---

## Steps

1. **Test connectivity to google.com**
   ```bash
   ping -c 4 google.com
Example output:

python
Copy
Edit
PING google.com (142.250.190.14) 56(84) bytes of data.
64 bytes from lhr25s47-in-f14.1e100.net (142.250.190.14): icmp_seq=1 ttl=118 time=14.5 ms
...
Display your network interface information and IP addresses

Modern systems:

bash
Copy
Edit
ip addr
Older systems:

bash
Copy
Edit
ifconfig
Example output (shortened):

sql
Copy
Edit
2: ens33: <BROADCAST,MULTICAST,UP,LOWER_UP> ...
    inet 192.168.1.100/24 brd 192.168.1.255 scope global dynamic ens33
Use curl to download the homepage of a website

bash
Copy
Edit
curl -o webpage.html https://example.com
Or using wget:

bash
Copy
Edit
wget -O webpage.html https://example.com
Verify the file was saved

bash
Copy
Edit
ls -l webpage.html
cat webpage.html | head -n 10
(Shows the first 10 lines of the downloaded HTML)
