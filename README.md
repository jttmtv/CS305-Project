# CS305-Project
**Start apache server**

`python3 ./netsim.py onelink start`

`python3 ./netsim.py sharelink start`

`python3 ./netsim.py twolink start`

**Start DNS server**

`python3 ./dns.py -s ../topology/onelink/onelink`

`python3 ./dns.py -s ../topology/sharelink/sharelink`

`python3 ./dns.py -s ../topology/twolink/twolink`

**Onelink: start proxies with default server port 15641 $(\alpha=0.1)$**

`python3 ./proxy.py -l ../logs/log1.txt -a 0.1 -p 8999 -d 5000 -s 15641`

`python3 ./proxy.py -l ../logs/log2.txt -a 0.1 -p 9000 -d 5000 -s 15641`

**Onelink: start proxies with default server port 15641 $(\alpha=0.5)$**

`python3 ./proxy.py -l ../logs/log1.txt -a 0.5 -p 8999 -d 5000 -s 15641`

`python3 ./proxy.py -l ../logs/log2.txt -a 0.5 -p 9000 -d 5000 -s 15641`

**Onelink: start proxies with default server port 15641 $(\alpha=0.9)$**

`python3 ./proxy.py -l ../logs/log1.txt -a 0.9 -p 8999 -d 5000 -s 15641`

`python3 ./proxy.py -l ../logs/log2.txt -a 0.9 -p 9000 -d 5000 -s 15641`

**Sharelink: start proxies with default server port 15640 and 15641 respectively $(\alpha=0.1)$**

`python3 ./proxy.py -l ../logs/log1.txt -a 0.1 -p 8999 -d 5000 -s 15640`

`python3 ./proxy.py -l ../logs/log2.txt -a 0.1 -p 9000 -d 5000 -s 15641`

**Sharelink: start proxies with default server port 15640 and 15641 respectively $(\alpha=0.5)$**

`python3 ./proxy.py -l ../logs/log1.txt -a 0.5 -p 8999 -d 5000 -s 15640`

`python3 ./proxy.py -l ../logs/log2.txt -a 0.5 -p 9000 -d 5000 -s 15641`

**Sharelink: start proxies with default server port 15640 and 15641 respectively $(\alpha=0.9)$**

`python3 ./proxy.py -l ../logs/log1.txt -a 0.9 -p 8999 -d 5000 -s 15640`

`python3 ./proxy.py -l ../logs/log2.txt -a 0.9 -p 9000 -d 5000 -s 15641`

**Twolink: start proxies with default server port 15640 and 15641 respectively $(\alpha=0.1)$**

`python3 ./proxy.py -l ../logs/log1.txt -a 0.1 -p 8999 -d 5000 -s 15640`

`python3 ./proxy.py -l ../logs/log2.txt -a 0.1 -p 9000 -d 5000 -s 15641`

**Twolink: start proxies with default server port 15640 and 15641 respectively $(\alpha=0.5)$**

`python3 ./proxy.py -l ../logs/log1.txt -a 0.5 -p 8999 -d 5000 -s 15640`

`python3 ./proxy.py -l ../logs/log2.txt -a 0.5 -p 9000 -d 5000 -s 15641`

**Twolink: start proxies with default server port 15640 and 15641 respectively $(\alpha=0.9)$**

`python3 ./proxy.py -l ../logs/log1.txt -a 0.9 -p 8999 -d 5000 -s 15640`

`python3 ./proxy.py -l ../logs/log2.txt -a 0.9 -p 9000 -d 5000 -s 15641`

**Trigger event**

`python3 netsim.py onelink run -e ./topology/onelink/onelink.events -l ./logs/log0.txt`

`python3 netsim.py sharelink run -e ./topology/sharelink/sharelink.events -l ./logs/log0.txt`

`python3 netsim.py twolink run -e ./topology/twolink/twolink.events -l ./logs/log0.txt`

**Web Browsers**

`http://127.0.0.1:8999/index.html`

`http://127.0.0.1:9000/index.html`

**Exit**

`http://127.0.0.1:8999/exit`

`http://127.0.0.1:9000/exit`

`python3 netsim.py onelink stop`

`python3 netsim.py sharelink stop`

`python3 netsim.py twolink stop`

**Grapher**

`python3 grapher.py ../logs/log0.txt ../logs/log1.txt ../logs/log2.txt`
