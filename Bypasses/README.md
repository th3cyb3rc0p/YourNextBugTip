# Bypasses
## Rate Limit Bypass

*[Tweet](https://twitter.com/ome_mishra/status/1241664059650404352) By [Ome Mishra](https://twitter.com/ome_mishra)*
```
Rate limiting Bypass by X-Host: 127.0.0.1 ..
If block after some request then try to increse the address from ...1 to ...2 and so on .
```

*[Tweet](https://twitter.com/udit_thakkur/status/1241832273898430464) By [Udit Thakkur](https://twitter.com/udit_thakkur/)*
```
Rate limit bypass:
Add header/s with request
X-Originating-IP: IP
X-Forwarded-For: IP
X-Remote-IP: IP
X-Remote-Addr: IP
X-Client-IP: IP
X-Host: IP
X-Forwared-Host: IP

If bypass successful, & after a while blocking request again. Increment the last octate
```

## Bypass Checks
*[Report #792895](https://hackerone.com/reports/792895) by [Green catz (hoangn1441)](https://hackerone.com/hoangn1441)*
- This trick can works for all kind of checks Old Password Check, Email Check, CSRF Token Check etc. :fire:

1. Change `parameter=value` to `parameter[]=value`
2. Bypass Successful

---------------------------------------------------------------------------------


