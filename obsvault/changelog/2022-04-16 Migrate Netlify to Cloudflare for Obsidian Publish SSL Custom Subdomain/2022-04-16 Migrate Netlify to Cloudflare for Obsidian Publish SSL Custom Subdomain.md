# 2022-04-16 Migrate Netlify to Cloudflare for Obsidian Publish SSL Custom Subdomain



Domain:
```
stevens.pro
```

Target Domain:
```
career.greg.stevens.pro
```

Obsidian Publish URL:




## Before
### Name servers

```
dns1.p07.nsone.net
dns2.p07.nsone.net
dns3.p07.nsone.net
dns4.p07.nsone.net
```



---
## Testing

https://www.stevens.pro/
https://stevens.pro/
https://greg.stevens.pro/
https://career.greg.stevens.pro/

*`career.` is the new [[Obsidian Publish]] Site*



---
## #DevDiary

### What's this?


![[career/images/Pasted image 20220416212213.png]]



> This zone is in a pending state and contains proxied records. Until the zone is activated, DNS queries to proxied records will expose the origin IP / hostname and traffic cannot be proxied through Cloudflare. For more information refer to [Limitations for pending domains](https://developers.cloudflare.com/dns/manage-dns-records/reference/proxied-dns-records#pending-domains).              




