# CS305-Project
**Start apache server**

`python3 ../netsim.py servers start -s ../servers/2servers`

**Start DNS server**

`python3 ./dns.py -s ../servers/2servers`

**Start proxy with default server port 8080**

`python3 ./proxy.py -l ../logs/log.txt -a 0.5 -p 8999 -d 5000 -s 8080`

**Start proxy without default server port**

`python3 ./proxy.py -l ../logs/log.txt -a 0.5 -p 8999 -d 5000`

**Web Browser**

`http://127.0.0.1:8999/index.html`

