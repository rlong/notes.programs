


list available ciphers:
```
nmap --script ssl-enum-ciphers -p 443 google.com
```

scan port 22 over a range of IPs:
```
nmap -p 22 10.11.6.1-255
```

scan port 22 over a range over a subnet:
```
nmap -p 22 192.168.1.0/24
nmap -p 22 10.11.6.0/24
```
