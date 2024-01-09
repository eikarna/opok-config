# TELKOMSEL CLOUDFRONT (2024)

## Type
Proxy-SSH WS

## Requirements
- SSH Server type CloudFront, SSH Port must be TLS (443, 8081, etc).
- Must enable "Pulsa Safe" / "Jaga Pulsa" Option in MyTelkomsel App.
- Set APN to Home (Many Province/State doesn't support this APN, tested at Jawa Barat) and wait until the signal comes to 4G/LTE.
- SSL Active.
- SNI Active.

### Payload
```php
GET / HTTP/1.1[crlf]Host: [host][crlf]Connection: Upgrade[crlf]User-Agent: [ua][crlf]Upgrade: websocket[crlf][crlf]
```

### Proxy
```php
18.161.49.87:80
18.161.49.87:443
18.161.49.45:80
18.161.49.45:443
18.67.172.129:80
18.67.172.129:443 (Recommended)
s3.digipos-prod.telkomsel.com:443
status.fb.com:443
```

### SNI
```txt
Same as SSH Server type CloudFront, but without Port.
```

## HowTo
1. Copy Payload, and paste it to Payload Input.
2. Copy SSH that you get, and paste it to SSH Input.
3. Wait until 4G/LTE, and Connect.
