# Modified Whatsapp-API
<p align='center'>
  <img src="https://files.catbox.moe/yno88s.jpg" width="360">
</p>

--- 

## Usage
```json
"depencies": {
  "@whiskeysockets/baileys": "github:Mutzxd99/BailsX"
}
```
## Import
```javascript
const {
  default:makeWASocket,
  // Other Options 
} = require('@whiskeysockets/baileys');
```

---
# How To Connect To Whatsapp
## With QR Code
```javascript
const {
  default: makeWASocket
} = require('@whiskeysockets/baileys');

const client = makeWASocket({
  browser: ['Ubuntu', 'Chrome', '20.00.1'],
  printQRInTerminal: true
})
```

## Connect With Number
```javascript
const {
  default: makeWASocket,
  fetchLatestWAWebVersion
} = require('@whiskeysockets/baileys');

const client = makeWASocket({
  browser: ['Ubuntu', 'Chrome', '20.00.1'],
  printQRInTerminal: false,
  version: fetchLatestWAWebVersion()
  // Other options
});

const number = "628XXXXX";
const code = await client.requestPairingCode(number.trim) /* Use : (number, "YYYYYYYY") for custom-pairing */

console.log("Ur pairing code : " + code)
```

## baileysCredits
```ThanksTo
@ZeppeliPdf - Owner Baileys
@Mutzxd - Remaking Baileys
@PutxzVoid - Sepuh Jir
```
