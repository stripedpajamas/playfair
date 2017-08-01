# Playfair

See [Playfair Cipher](https://en.wikipedia.org/wiki/Playfair_cipher) on Wikiepdia.

Merges `i` and `j`, uses `x` as a pad. 

Example usage:
```javascript
const Playfair = require('./playfair');
  
const pf = new Playfair();
pf.setKey('my secret key');
  
// encrypt:
pf.process({ input: 'tomato basil marinara' }); // KNECKNHCMOIYCTLOCTHE
  
// decrypt:
pf.process({ input: 'KNECKNHCMOIYCTLOCTHE', decrypt: true }); // TOMATOBASILMARINARAX

```