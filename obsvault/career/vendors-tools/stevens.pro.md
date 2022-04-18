# stevens.pro - Change DNS Host from Netlify to Cloudflare 2022-04-16




Domain Registrar

https://www.domainpeople.com/userAdmin/Account?PartnerID=startsite&SiteID=startsite07us&language=en






Domain Name: stevens.pro
Registry Domain ID: 0864767f06124b6abb832b5841a7af97-DONUTS
Registrar WHOIS Server: whois.domainpeople.com
Registrar URL: http://www.domainpeople.com/
Updated Date: 2020-12-27T06:04:44Z
Creation Date: 2009-01-05T00:00:00Z
Registry Expiry Date: 2026-01-05T00:00:00Z




Domain Name: stevens.pro Registry Domain ID: 0864767f06124b6abb832b5841a7af97-DONUTS Registrar WHOIS Server: whois.domainpeople.com Registrar URL: http://www.domainpeople.com/ Updated Date: 2020-12-27T06:04:44Z Creation Date: 2009-01-05T00:00:00Z Registry Expiry Date: 2026-01-05T00:00:00ZDomain Name: stevens.pro Registry Domain ID: 0864767f06124b6abb832b5841a7af97-DONUTS Registrar WHOIS Server: whois.domainpeople.com Registrar URL: http://www.domainpeople.com/ Updated Date: 2020-12-27T06:04:44Z Creation Date: 2009-01-05T00:00:00Z Registry Expiry Date: 2026-01-05T00:00:00Z



---
From DomainPeople.com:

> **Note :** Your domain name is registered with a reseller or has been moved to DomainPeople's new hosting platform. To gain access to your account please [log in here](https://sitecontrol-sp.hostway.com/)


[SiteControl (hostway.com)](https://sitecontrol-sp.hostway.com/SiteControl/R03150815/plugins/commons/init.tile)


#before



---



### Test
```shell
curl -I greg.stevens.pro
curl -I stevens.pro
curl -I www.stevens.pro
curl -I https://stevens.pro
curl -I https://www.stevens.pro
curl -I https://career.greg.stevens.pro
```

#script #Windows #Linux #ProTip #TheMoreYouKnow



#### Test Output - Before Change
- Tested while nameservers were updating.
- Was the results of older Netlify records.
- Consider it the #before output.
- Changing just to get a custom domain for this vault `career.greg.stevens.pro`.
- Need the Cloudflare SSL wrapper.
- Or I could use the default domain - `publish.obsidian.md/greg-stevens-career/`. Nah.

```shell

gsteve@benny-win MSYS ~
$ curl -I greg.stevens.pro
HTTP/1.1 301 Moved Permanently
Age: 0
Cache-Control: public, max-age=0, must-revalidate
Content-Length: 40
Content-Type: text/plain
Date: Sun, 17 Apr 2022 04:46:18 GMT
Location: https://greg.stevens.pro/
Server: Netlify
X-Nf-Request-Id: 01G0TXFMF8Y40172302XV8CSP2


gsteve@benny-win MSYS ~
$ curl -I stevens.pro
HTTP/1.1 301 Moved Permanently
Age: 70103
Cache-Control: public, max-age=0, must-revalidate
Content-Length: 35
Content-Type: text/plain
Date: Sat, 16 Apr 2022 09:17:59 GMT
Location: https://stevens.pro/
Server: Netlify
X-Nf-Request-Id: 01G0TXFRCJRGCH6J4XFSY38JQ9


gsteve@benny-win MSYS ~
$ curl -I www.stevens.pro
HTTP/1.1 301 Moved Permanently
Age: 0
Cache-Control: public, max-age=0, must-revalidate
Content-Length: 39
Content-Type: text/plain
Date: Sun, 17 Apr 2022 04:46:25 GMT
Location: https://www.stevens.pro/
Server: Netlify
X-Nf-Request-Id: 01G0TXFVVKNCBBQP1SJEEPS4NZ


gsteve@benny-win MSYS ~
$ curl -I https://stevens.pro
HTTP/1.1 301 Moved Permanently
Age: 70112
Cache-Control: public, max-age=0, must-revalidate
Content-Length: 39
Content-Type: text/plain
Date: Sat, 16 Apr 2022 09:18:01 GMT
Location: https://www.stevens.pro/
Server: Netlify
Strict-Transport-Security: max-age=31536000
X-Nf-Request-Id: 01G0TXG35X1HXT6DSWAE0RWBJ1


gsteve@benny-win MSYS ~
$ curl -I https://www.stevens.pro
HTTP/1.1 200 OK
Age: 0
Cache-Control: public, max-age=0, must-revalidate
Content-Type: text/html; charset=UTF-8
Date: Sun, 17 Apr 2022 04:46:38 GMT
Etag: "f3bed69f6c77885450d7e661123855be-ssl"
Server: Netlify
Strict-Transport-Security: max-age=31536000
X-Nf-Request-Id: 01G0TXG875WMQVBPT1J6B7QXP4


gsteve@benny-win MSYS ~
$ curl -I https://career.greg.stevens.pro
curl: (6) Could not resolve host: career.greg.stevens.pro

gsteve@benny-win MSYS ~
$ nslookup
Default Server:  node-1w7jr9n24twqzs2cg5ed4tjl3.ipv6.telus.net
Address:  2001:568:ff09:10c::67

> server logan.ns.cloudflare.com
Default Server:  logan.ns.cloudflare.com
Addresses:  2606:4700:58::adf5:3bc6
          2a06:98c1:50::ac40:21c6
          2803:f800:50::6ca2:c1c6
          172.64.33.198
          108.162.193.198
          173.245.59.198

> greg.stevens.pro
Server:  logan.ns.cloudflare.com
Addresses:  2606:4700:58::adf5:3bc6
          2a06:98c1:50::ac40:21c6
          2803:f800:50::6ca2:c1c6
          172.64.33.198
          108.162.193.198
          173.245.59.198

Name:    greg.stevens.pro

> stevens.pro
Server:  logan.ns.cloudflare.com
Addresses:  2606:4700:58::adf5:3bc6
          2a06:98c1:50::ac40:21c6
          2803:f800:50::6ca2:c1c6
          172.64.33.198
          108.162.193.198
          173.245.59.198

Name:    stevens.pro
Addresses:  99.83.231.61
          75.2.60.5

> www.stevens.pro
Server:  logan.ns.cloudflare.com
Addresses:  2606:4700:58::adf5:3bc6
          2a06:98c1:50::ac40:21c6
          2803:f800:50::6ca2:c1c6
          172.64.33.198
          108.162.193.198
          173.245.59.198

Name:    www.stevens.pro

> career.greg.stevens.pro
Server:  logan.ns.cloudflare.com
Addresses:  2606:4700:58::adf5:3bc6
          2a06:98c1:50::ac40:21c6
          2803:f800:50::6ca2:c1c6
          172.64.33.198
          108.162.193.198
          173.245.59.198

*** logan.ns.cloudflare.com can't find career.greg.stevens.pro: Non-existent domain
> career.greg.stevens.pro
gsteve@benny-win MSYS ~
$ quit
bash: quit: command not found

gsteve@benny-win MSYS ~
$ curl -I https://www.stevens.pro^C

gsteve@benny-win MSYS ~
$ history -w

gsteve@benny-win MSYS ~
$ cat ~/.bash_history
```
