# QRcode Scanner

QR Code scanner for login hotspot MikroTik

## How to use

1. Add url button to login page
```
<button onclick="window.location='https://hotspotbilling.github.io/qrlogin/?hotspot=Your company&back=encoded url for back to login';">QR Login</button>
```
2. Add walled garden, run this script in MikroTik terminal.
```
/ip hotspot walled-garden ip
add action=accept comment="QR Code Scanner" disabled=no dst-host=hotspotbilling.github.io
```
