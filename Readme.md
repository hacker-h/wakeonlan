# Wakeonelan
This is a simple python alpine based docker image with the wakeonlan tool installed.

# Usage
```
docker run hackerh/wakeonlan wakeonlan -i <BROADCAST_IP> -p <PORT> <MAC_ADDRESS>
```

# Example Usage
```
docker run hackerh/wakeonlan wakeonlan -i 192.168.0.255 -p 9 25:3E:BF:3E:28:D9
```
