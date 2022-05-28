# CS305-Project
**Start apache server**

`cd src && python3 ../netsim.py servers start -s ../servers/2servers`

**Start DNS server**

`python3 ./dns.py -s ../servers/2servers`

**Start proxy with default server port 8080**

`cd src && python3 ./proxy.py -l ../logs/log.txt -a 0.5 -p 8999 -d 5000 -s 8080`

**Start proxy without default server port**

`cd src && python3 ./proxy.py -l ../logs/log.txt -a 0.5 -p 8999 -d 5000`

**Web Browser**

`http://localhost:8999/index.html`

