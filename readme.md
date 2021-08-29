# IETTS Lib

# Installing

```bash
npm install @yek-plus/ietts
```

# Usage

```js
const ietts = require("@yek-plus/ietts");
ietts().get({ iettsNo: 3700001 }).then(console.log);
```

# Options

| property | type       | required | default            | description            |
| -------- | ---------- | -------- | ------------------ | ---------------------- |
| fetch    | `function` | false    | node-fetch package | request fetch function |

# Methods

## get

### Input

| property | type     | required | default | description                                                      |
| -------- | -------- | -------- | ------- | ---------------------------------------------------------------- |
| iettsNo  | `number` | true     | null    | İkinci El Motorlu Kara Taşıtları Ticareti Bilgi Sistemi Numarası |

### Response

```js
{
  status: Boolean,
  error: String,
  doc: {
    belgeNo: String,
    belgeTarihi: String,
    belgeDurumu: String,
    belgeDurumuBool: Boolean,
    isletmeAdi: String,
    isletmeSahibi: String,
    isletmeAdres: String,
  },
};
```

# Todo

- [ ] Write Tests
