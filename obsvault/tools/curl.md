# curl

## #HowTo View Request Headers with the `-I` Option
#ProTip  #Windows #Linux #ComputerNetwork

```
curl -I 
```


### #Example Testing Multiple Sites


#### #CommandHistory
```shell
curl -I greg.stevens.pro
curl -I stevens.pro
curl -I www.stevens.pro
curl -I https://stevens.pro
curl -I https://www.stevens.pro
curl -I https://career.greg.stevens.pro
```

#### Results

- Note, using no `https://` on purpose.
- Web server, or Cloudflare, should respond with a [[301 Redirect]] to the #https site.
- Let's see...
- Running this in [[Windows Terminal]] of course.

```
curl -I career.greg.stevens.pro
```

