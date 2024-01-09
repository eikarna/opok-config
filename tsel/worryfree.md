# TELKOMSEL WORRYFREE (2024)

## Type
Direct-SSH WS

## Requirements
- SSH Server, recommended Dropbear instead OpenSSH.
- Must enable "Pulsa Safe"/"Jaga Pulsa" Option in MyTelkomsel App.
- Set APN to Home (Many Province/State doesn't support this APN, tested at Jawa Barat) and wait until the signal comes to 4G/LTE.
- Patient.

### Payload
```php
GET /worryfree HTTP/1.1[crlf]Host: tsel.me[crlf]Connection: Upgrade[crlf]Upgrade: websocket[crlf]User-Agent: [ua][crlf][crlf]
```

## HowTo
1. Copy Payload, and paste it to Payload Input.
2. Copy SSH that you get, and paste it to SSH Input.
3. Wait until 4G/LTE, and Connect.
