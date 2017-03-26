# api documentation for  [crypto-js (v3.1.8)](http://github.com/brix/crypto-js)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-crypto-js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-crypto-js)
#### JavaScript library of crypto standards.

[![NPM](https://nodei.co/npm/crypto-js.png?downloads=true)](https://www.npmjs.com/package/crypto-js)

[![apidoc](https://npmdoc.github.io/node-npmdoc-crypto-js/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-crypto-js_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-crypto-js/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-crypto-js/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Evan Vosberg",
        "url": "http://github.com/evanvosberg"
    },
    "bugs": {
        "url": "https://github.com/brix/crypto-js/issues"
    },
    "dependencies": {},
    "description": "JavaScript library of crypto standards.",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "715f070bf6014f2ae992a98b3929258b713f08d5",
        "tarball": "https://registry.npmjs.org/crypto-js/-/crypto-js-3.1.8.tgz"
    },
    "gitHead": "be8d44d18736f438ca480664d7d8bea46f117b5a",
    "homepage": "http://github.com/brix/crypto-js",
    "keywords": [
        "security",
        "crypto",
        "Hash",
        "MD5",
        "SHA1",
        "SHA-1",
        "SHA256",
        "SHA-256",
        "RC4",
        "Rabbit",
        "AES",
        "DES",
        "PBKDF2",
        "HMAC",
        "OFB",
        "CFB",
        "CTR",
        "CBC",
        "Base64"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "evanvosberg",
            "email": "evanvosberg@inext.me"
        }
    ],
    "name": "crypto-js",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/brix/crypto-js.git"
    },
    "scripts": {},
    "version": "3.1.8"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module crypto-js](#apidoc.module.crypto-js)
1.  [function <span class="apidocSignatureSpan">crypto-js.</span>EvpKDF (password, salt, cfg)](#apidoc.element.crypto-js.EvpKDF)
1.  [function <span class="apidocSignatureSpan">crypto-js.</span>HmacMD5 (message, key)](#apidoc.element.crypto-js.HmacMD5)
1.  [function <span class="apidocSignatureSpan">crypto-js.</span>HmacRIPEMD160 (message, key)](#apidoc.element.crypto-js.HmacRIPEMD160)
1.  [function <span class="apidocSignatureSpan">crypto-js.</span>HmacSHA1 (message, key)](#apidoc.element.crypto-js.HmacSHA1)
1.  [function <span class="apidocSignatureSpan">crypto-js.</span>HmacSHA224 (message, key)](#apidoc.element.crypto-js.HmacSHA224)
1.  [function <span class="apidocSignatureSpan">crypto-js.</span>HmacSHA256 (message, key)](#apidoc.element.crypto-js.HmacSHA256)
1.  [function <span class="apidocSignatureSpan">crypto-js.</span>HmacSHA3 (message, key)](#apidoc.element.crypto-js.HmacSHA3)
1.  [function <span class="apidocSignatureSpan">crypto-js.</span>HmacSHA384 (message, key)](#apidoc.element.crypto-js.HmacSHA384)
1.  [function <span class="apidocSignatureSpan">crypto-js.</span>HmacSHA512 (message, key)](#apidoc.element.crypto-js.HmacSHA512)
1.  [function <span class="apidocSignatureSpan">crypto-js.</span>MD5 (message, cfg)](#apidoc.element.crypto-js.MD5)
1.  [function <span class="apidocSignatureSpan">crypto-js.</span>PBKDF2 (password, salt, cfg)](#apidoc.element.crypto-js.PBKDF2)
1.  [function <span class="apidocSignatureSpan">crypto-js.</span>RIPEMD160 (message, cfg)](#apidoc.element.crypto-js.RIPEMD160)
1.  [function <span class="apidocSignatureSpan">crypto-js.</span>SHA1 (message, cfg)](#apidoc.element.crypto-js.SHA1)
1.  [function <span class="apidocSignatureSpan">crypto-js.</span>SHA224 (message, cfg)](#apidoc.element.crypto-js.SHA224)
1.  [function <span class="apidocSignatureSpan">crypto-js.</span>SHA256 (message, cfg)](#apidoc.element.crypto-js.SHA256)
1.  [function <span class="apidocSignatureSpan">crypto-js.</span>SHA3 (message, cfg)](#apidoc.element.crypto-js.SHA3)
1.  [function <span class="apidocSignatureSpan">crypto-js.</span>SHA384 (message, cfg)](#apidoc.element.crypto-js.SHA384)
1.  [function <span class="apidocSignatureSpan">crypto-js.</span>SHA512 (message, cfg)](#apidoc.element.crypto-js.SHA512)
1.  object <span class="apidocSignatureSpan">crypto-js.</span>AES
1.  object <span class="apidocSignatureSpan">crypto-js.</span>DES
1.  object <span class="apidocSignatureSpan">crypto-js.</span>RC4
1.  object <span class="apidocSignatureSpan">crypto-js.</span>RC4Drop
1.  object <span class="apidocSignatureSpan">crypto-js.</span>Rabbit
1.  object <span class="apidocSignatureSpan">crypto-js.</span>RabbitLegacy
1.  object <span class="apidocSignatureSpan">crypto-js.</span>TripleDES
1.  object <span class="apidocSignatureSpan">crypto-js.</span>algo
1.  object <span class="apidocSignatureSpan">crypto-js.</span>enc
1.  object <span class="apidocSignatureSpan">crypto-js.</span>format
1.  object <span class="apidocSignatureSpan">crypto-js.</span>kdf
1.  object <span class="apidocSignatureSpan">crypto-js.</span>lib
1.  object <span class="apidocSignatureSpan">crypto-js.</span>mode
1.  object <span class="apidocSignatureSpan">crypto-js.</span>pad
1.  object <span class="apidocSignatureSpan">crypto-js.</span>x64

#### [module crypto-js.AES](#apidoc.module.crypto-js.AES)
1.  [function <span class="apidocSignatureSpan">crypto-js.AES.</span>decrypt (ciphertext, key, cfg)](#apidoc.element.crypto-js.AES.decrypt)
1.  [function <span class="apidocSignatureSpan">crypto-js.AES.</span>encrypt (message, key, cfg)](#apidoc.element.crypto-js.AES.encrypt)

#### [module crypto-js.DES](#apidoc.module.crypto-js.DES)
1.  [function <span class="apidocSignatureSpan">crypto-js.DES.</span>decrypt (ciphertext, key, cfg)](#apidoc.element.crypto-js.DES.decrypt)
1.  [function <span class="apidocSignatureSpan">crypto-js.DES.</span>encrypt (message, key, cfg)](#apidoc.element.crypto-js.DES.encrypt)

#### [module crypto-js.RC4](#apidoc.module.crypto-js.RC4)
1.  [function <span class="apidocSignatureSpan">crypto-js.RC4.</span>decrypt (ciphertext, key, cfg)](#apidoc.element.crypto-js.RC4.decrypt)
1.  [function <span class="apidocSignatureSpan">crypto-js.RC4.</span>encrypt (message, key, cfg)](#apidoc.element.crypto-js.RC4.encrypt)

#### [module crypto-js.RC4Drop](#apidoc.module.crypto-js.RC4Drop)
1.  [function <span class="apidocSignatureSpan">crypto-js.RC4Drop.</span>decrypt (ciphertext, key, cfg)](#apidoc.element.crypto-js.RC4Drop.decrypt)
1.  [function <span class="apidocSignatureSpan">crypto-js.RC4Drop.</span>encrypt (message, key, cfg)](#apidoc.element.crypto-js.RC4Drop.encrypt)

#### [module crypto-js.Rabbit](#apidoc.module.crypto-js.Rabbit)
1.  [function <span class="apidocSignatureSpan">crypto-js.Rabbit.</span>decrypt (ciphertext, key, cfg)](#apidoc.element.crypto-js.Rabbit.decrypt)
1.  [function <span class="apidocSignatureSpan">crypto-js.Rabbit.</span>encrypt (message, key, cfg)](#apidoc.element.crypto-js.Rabbit.encrypt)

#### [module crypto-js.RabbitLegacy](#apidoc.module.crypto-js.RabbitLegacy)
1.  [function <span class="apidocSignatureSpan">crypto-js.RabbitLegacy.</span>decrypt (ciphertext, key, cfg)](#apidoc.element.crypto-js.RabbitLegacy.decrypt)
1.  [function <span class="apidocSignatureSpan">crypto-js.RabbitLegacy.</span>encrypt (message, key, cfg)](#apidoc.element.crypto-js.RabbitLegacy.encrypt)

#### [module crypto-js.TripleDES](#apidoc.module.crypto-js.TripleDES)
1.  [function <span class="apidocSignatureSpan">crypto-js.TripleDES.</span>decrypt (ciphertext, key, cfg)](#apidoc.element.crypto-js.TripleDES.decrypt)
1.  [function <span class="apidocSignatureSpan">crypto-js.TripleDES.</span>encrypt (message, key, cfg)](#apidoc.element.crypto-js.TripleDES.encrypt)



# <a name="apidoc.module.crypto-js"></a>[module crypto-js](#apidoc.module.crypto-js)

#### <a name="apidoc.element.crypto-js.EvpKDF"></a>[function <span class="apidocSignatureSpan">crypto-js.</span>EvpKDF (password, salt, cfg)](#apidoc.element.crypto-js.EvpKDF)
- description and source-code
```javascript
EvpKDF = function (password, salt, cfg) {
	        return EvpKDF.create(cfg).compute(password, salt);
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-js.HmacMD5"></a>[function <span class="apidocSignatureSpan">crypto-js.</span>HmacMD5 (message, key)](#apidoc.element.crypto-js.HmacMD5)
- description and source-code
```javascript
HmacMD5 = function (message, key) {
	                return new C_algo.HMAC.init(hasher, key).finalize(message);
	            }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-js.HmacRIPEMD160"></a>[function <span class="apidocSignatureSpan">crypto-js.</span>HmacRIPEMD160 (message, key)](#apidoc.element.crypto-js.HmacRIPEMD160)
- description and source-code
```javascript
HmacRIPEMD160 = function (message, key) {
	                return new C_algo.HMAC.init(hasher, key).finalize(message);
	            }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-js.HmacSHA1"></a>[function <span class="apidocSignatureSpan">crypto-js.</span>HmacSHA1 (message, key)](#apidoc.element.crypto-js.HmacSHA1)
- description and source-code
```javascript
HmacSHA1 = function (message, key) {
	                return new C_algo.HMAC.init(hasher, key).finalize(message);
	            }
```
- example usage
```shell
...
console.log(SHA256("Message"));
'''

Including all libraries, for access to extra methods:

'''javascript
var CryptoJS = require("crypto-js");
console.log(CryptoJS.HmacSHA1("Message", "Key"));
'''

## Client (browser)

Requirements:

- Node.js
...
```

#### <a name="apidoc.element.crypto-js.HmacSHA224"></a>[function <span class="apidocSignatureSpan">crypto-js.</span>HmacSHA224 (message, key)](#apidoc.element.crypto-js.HmacSHA224)
- description and source-code
```javascript
HmacSHA224 = function (message, key) {
	                return new C_algo.HMAC.init(hasher, key).finalize(message);
	            }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-js.HmacSHA256"></a>[function <span class="apidocSignatureSpan">crypto-js.</span>HmacSHA256 (message, key)](#apidoc.element.crypto-js.HmacSHA256)
- description and source-code
```javascript
HmacSHA256 = function (message, key) {
	                return new C_algo.HMAC.init(hasher, key).finalize(message);
	            }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-js.HmacSHA3"></a>[function <span class="apidocSignatureSpan">crypto-js.</span>HmacSHA3 (message, key)](#apidoc.element.crypto-js.HmacSHA3)
- description and source-code
```javascript
HmacSHA3 = function (message, key) {
	                return new C_algo.HMAC.init(hasher, key).finalize(message);
	            }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-js.HmacSHA384"></a>[function <span class="apidocSignatureSpan">crypto-js.</span>HmacSHA384 (message, key)](#apidoc.element.crypto-js.HmacSHA384)
- description and source-code
```javascript
HmacSHA384 = function (message, key) {
	                return new C_algo.HMAC.init(hasher, key).finalize(message);
	            }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-js.HmacSHA512"></a>[function <span class="apidocSignatureSpan">crypto-js.</span>HmacSHA512 (message, key)](#apidoc.element.crypto-js.HmacSHA512)
- description and source-code
```javascript
HmacSHA512 = function (message, key) {
	                return new C_algo.HMAC.init(hasher, key).finalize(message);
	            }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-js.MD5"></a>[function <span class="apidocSignatureSpan">crypto-js.</span>MD5 (message, cfg)](#apidoc.element.crypto-js.MD5)
- description and source-code
```javascript
MD5 = function (message, cfg) {
	                return new hasher.init(cfg).finalize(message);
	            }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-js.PBKDF2"></a>[function <span class="apidocSignatureSpan">crypto-js.</span>PBKDF2 (password, salt, cfg)](#apidoc.element.crypto-js.PBKDF2)
- description and source-code
```javascript
PBKDF2 = function (password, salt, cfg) {
	        return PBKDF2.create(cfg).compute(password, salt);
	    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-js.RIPEMD160"></a>[function <span class="apidocSignatureSpan">crypto-js.</span>RIPEMD160 (message, cfg)](#apidoc.element.crypto-js.RIPEMD160)
- description and source-code
```javascript
RIPEMD160 = function (message, cfg) {
	                return new hasher.init(cfg).finalize(message);
	            }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-js.SHA1"></a>[function <span class="apidocSignatureSpan">crypto-js.</span>SHA1 (message, cfg)](#apidoc.element.crypto-js.SHA1)
- description and source-code
```javascript
SHA1 = function (message, cfg) {
	                return new hasher.init(cfg).finalize(message);
	            }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-js.SHA224"></a>[function <span class="apidocSignatureSpan">crypto-js.</span>SHA224 (message, cfg)](#apidoc.element.crypto-js.SHA224)
- description and source-code
```javascript
SHA224 = function (message, cfg) {
	                return new hasher.init(cfg).finalize(message);
	            }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-js.SHA256"></a>[function <span class="apidocSignatureSpan">crypto-js.</span>SHA256 (message, cfg)](#apidoc.element.crypto-js.SHA256)
- description and source-code
```javascript
SHA256 = function (message, cfg) {
	                return new hasher.init(cfg).finalize(message);
	            }
```
- example usage
```shell
...

### Usage without RequireJS

'''html
<script type="text/javascript" src="path-to/bower_components/crypto-js/crypto-js.js"></script>
<script type="text/javascript">
    var encrypted = CryptoJS.AES(...);
    var encrypted = CryptoJS.SHA256(...);
</script>
'''

## API

See: https://code.google.com/p/crypto-js
...
```

#### <a name="apidoc.element.crypto-js.SHA3"></a>[function <span class="apidocSignatureSpan">crypto-js.</span>SHA3 (message, cfg)](#apidoc.element.crypto-js.SHA3)
- description and source-code
```javascript
SHA3 = function (message, cfg) {
	                return new hasher.init(cfg).finalize(message);
	            }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-js.SHA384"></a>[function <span class="apidocSignatureSpan">crypto-js.</span>SHA384 (message, cfg)](#apidoc.element.crypto-js.SHA384)
- description and source-code
```javascript
SHA384 = function (message, cfg) {
	                return new hasher.init(cfg).finalize(message);
	            }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.crypto-js.SHA512"></a>[function <span class="apidocSignatureSpan">crypto-js.</span>SHA512 (message, cfg)](#apidoc.element.crypto-js.SHA512)
- description and source-code
```javascript
SHA512 = function (message, cfg) {
	                return new hasher.init(cfg).finalize(message);
	            }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.crypto-js.AES"></a>[module crypto-js.AES](#apidoc.module.crypto-js.AES)

#### <a name="apidoc.element.crypto-js.AES.decrypt"></a>[function <span class="apidocSignatureSpan">crypto-js.AES.</span>decrypt (ciphertext, key, cfg)](#apidoc.element.crypto-js.AES.decrypt)
- description and source-code
```javascript
decrypt = function (ciphertext, key, cfg) {
	                        return selectCipherStrategy(key).decrypt(cipher, ciphertext, key, cfg);
	                    }
```
- example usage
```shell
...
'''javascript
var CryptoJS = require("crypto-js");

// Encrypt
var ciphertext = CryptoJS.AES.encrypt('my message', 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var plaintext = bytes.toString(CryptoJS.enc.Utf8);

console.log(plaintext);
'''

#### Object encryption
...
```

#### <a name="apidoc.element.crypto-js.AES.encrypt"></a>[function <span class="apidocSignatureSpan">crypto-js.AES.</span>encrypt (message, key, cfg)](#apidoc.element.crypto-js.AES.encrypt)
- description and source-code
```javascript
encrypt = function (message, key, cfg) {
	                        return selectCipherStrategy(key).encrypt(cipher, message, key, cfg);
	                    }
```
- example usage
```shell
...

#### Plain text encryption

'''javascript
var CryptoJS = require("crypto-js");

// Encrypt
var ciphertext = CryptoJS.AES.encrypt('my message', 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var plaintext = bytes.toString(CryptoJS.enc.Utf8);

console.log(plaintext);
'''
...
```



# <a name="apidoc.module.crypto-js.DES"></a>[module crypto-js.DES](#apidoc.module.crypto-js.DES)

#### <a name="apidoc.element.crypto-js.DES.decrypt"></a>[function <span class="apidocSignatureSpan">crypto-js.DES.</span>decrypt (ciphertext, key, cfg)](#apidoc.element.crypto-js.DES.decrypt)
- description and source-code
```javascript
decrypt = function (ciphertext, key, cfg) {
	                        return selectCipherStrategy(key).decrypt(cipher, ciphertext, key, cfg);
	                    }
```
- example usage
```shell
...
'''javascript
var CryptoJS = require("crypto-js");

// Encrypt
var ciphertext = CryptoJS.AES.encrypt('my message', 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var plaintext = bytes.toString(CryptoJS.enc.Utf8);

console.log(plaintext);
'''

#### Object encryption
...
```

#### <a name="apidoc.element.crypto-js.DES.encrypt"></a>[function <span class="apidocSignatureSpan">crypto-js.DES.</span>encrypt (message, key, cfg)](#apidoc.element.crypto-js.DES.encrypt)
- description and source-code
```javascript
encrypt = function (message, key, cfg) {
	                        return selectCipherStrategy(key).encrypt(cipher, message, key, cfg);
	                    }
```
- example usage
```shell
...

#### Plain text encryption

'''javascript
var CryptoJS = require("crypto-js");

// Encrypt
var ciphertext = CryptoJS.AES.encrypt('my message', 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var plaintext = bytes.toString(CryptoJS.enc.Utf8);

console.log(plaintext);
'''
...
```



# <a name="apidoc.module.crypto-js.RC4"></a>[module crypto-js.RC4](#apidoc.module.crypto-js.RC4)

#### <a name="apidoc.element.crypto-js.RC4.decrypt"></a>[function <span class="apidocSignatureSpan">crypto-js.RC4.</span>decrypt (ciphertext, key, cfg)](#apidoc.element.crypto-js.RC4.decrypt)
- description and source-code
```javascript
decrypt = function (ciphertext, key, cfg) {
	                        return selectCipherStrategy(key).decrypt(cipher, ciphertext, key, cfg);
	                    }
```
- example usage
```shell
...
'''javascript
var CryptoJS = require("crypto-js");

// Encrypt
var ciphertext = CryptoJS.AES.encrypt('my message', 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var plaintext = bytes.toString(CryptoJS.enc.Utf8);

console.log(plaintext);
'''

#### Object encryption
...
```

#### <a name="apidoc.element.crypto-js.RC4.encrypt"></a>[function <span class="apidocSignatureSpan">crypto-js.RC4.</span>encrypt (message, key, cfg)](#apidoc.element.crypto-js.RC4.encrypt)
- description and source-code
```javascript
encrypt = function (message, key, cfg) {
	                        return selectCipherStrategy(key).encrypt(cipher, message, key, cfg);
	                    }
```
- example usage
```shell
...

#### Plain text encryption

'''javascript
var CryptoJS = require("crypto-js");

// Encrypt
var ciphertext = CryptoJS.AES.encrypt('my message', 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var plaintext = bytes.toString(CryptoJS.enc.Utf8);

console.log(plaintext);
'''
...
```



# <a name="apidoc.module.crypto-js.RC4Drop"></a>[module crypto-js.RC4Drop](#apidoc.module.crypto-js.RC4Drop)

#### <a name="apidoc.element.crypto-js.RC4Drop.decrypt"></a>[function <span class="apidocSignatureSpan">crypto-js.RC4Drop.</span>decrypt (ciphertext, key, cfg)](#apidoc.element.crypto-js.RC4Drop.decrypt)
- description and source-code
```javascript
decrypt = function (ciphertext, key, cfg) {
	                        return selectCipherStrategy(key).decrypt(cipher, ciphertext, key, cfg);
	                    }
```
- example usage
```shell
...
'''javascript
var CryptoJS = require("crypto-js");

// Encrypt
var ciphertext = CryptoJS.AES.encrypt('my message', 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var plaintext = bytes.toString(CryptoJS.enc.Utf8);

console.log(plaintext);
'''

#### Object encryption
...
```

#### <a name="apidoc.element.crypto-js.RC4Drop.encrypt"></a>[function <span class="apidocSignatureSpan">crypto-js.RC4Drop.</span>encrypt (message, key, cfg)](#apidoc.element.crypto-js.RC4Drop.encrypt)
- description and source-code
```javascript
encrypt = function (message, key, cfg) {
	                        return selectCipherStrategy(key).encrypt(cipher, message, key, cfg);
	                    }
```
- example usage
```shell
...

#### Plain text encryption

'''javascript
var CryptoJS = require("crypto-js");

// Encrypt
var ciphertext = CryptoJS.AES.encrypt('my message', 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var plaintext = bytes.toString(CryptoJS.enc.Utf8);

console.log(plaintext);
'''
...
```



# <a name="apidoc.module.crypto-js.Rabbit"></a>[module crypto-js.Rabbit](#apidoc.module.crypto-js.Rabbit)

#### <a name="apidoc.element.crypto-js.Rabbit.decrypt"></a>[function <span class="apidocSignatureSpan">crypto-js.Rabbit.</span>decrypt (ciphertext, key, cfg)](#apidoc.element.crypto-js.Rabbit.decrypt)
- description and source-code
```javascript
decrypt = function (ciphertext, key, cfg) {
	                        return selectCipherStrategy(key).decrypt(cipher, ciphertext, key, cfg);
	                    }
```
- example usage
```shell
...
'''javascript
var CryptoJS = require("crypto-js");

// Encrypt
var ciphertext = CryptoJS.AES.encrypt('my message', 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var plaintext = bytes.toString(CryptoJS.enc.Utf8);

console.log(plaintext);
'''

#### Object encryption
...
```

#### <a name="apidoc.element.crypto-js.Rabbit.encrypt"></a>[function <span class="apidocSignatureSpan">crypto-js.Rabbit.</span>encrypt (message, key, cfg)](#apidoc.element.crypto-js.Rabbit.encrypt)
- description and source-code
```javascript
encrypt = function (message, key, cfg) {
	                        return selectCipherStrategy(key).encrypt(cipher, message, key, cfg);
	                    }
```
- example usage
```shell
...

#### Plain text encryption

'''javascript
var CryptoJS = require("crypto-js");

// Encrypt
var ciphertext = CryptoJS.AES.encrypt('my message', 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var plaintext = bytes.toString(CryptoJS.enc.Utf8);

console.log(plaintext);
'''
...
```



# <a name="apidoc.module.crypto-js.RabbitLegacy"></a>[module crypto-js.RabbitLegacy](#apidoc.module.crypto-js.RabbitLegacy)

#### <a name="apidoc.element.crypto-js.RabbitLegacy.decrypt"></a>[function <span class="apidocSignatureSpan">crypto-js.RabbitLegacy.</span>decrypt (ciphertext, key, cfg)](#apidoc.element.crypto-js.RabbitLegacy.decrypt)
- description and source-code
```javascript
decrypt = function (ciphertext, key, cfg) {
	                        return selectCipherStrategy(key).decrypt(cipher, ciphertext, key, cfg);
	                    }
```
- example usage
```shell
...
'''javascript
var CryptoJS = require("crypto-js");

// Encrypt
var ciphertext = CryptoJS.AES.encrypt('my message', 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var plaintext = bytes.toString(CryptoJS.enc.Utf8);

console.log(plaintext);
'''

#### Object encryption
...
```

#### <a name="apidoc.element.crypto-js.RabbitLegacy.encrypt"></a>[function <span class="apidocSignatureSpan">crypto-js.RabbitLegacy.</span>encrypt (message, key, cfg)](#apidoc.element.crypto-js.RabbitLegacy.encrypt)
- description and source-code
```javascript
encrypt = function (message, key, cfg) {
	                        return selectCipherStrategy(key).encrypt(cipher, message, key, cfg);
	                    }
```
- example usage
```shell
...

#### Plain text encryption

'''javascript
var CryptoJS = require("crypto-js");

// Encrypt
var ciphertext = CryptoJS.AES.encrypt('my message', 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var plaintext = bytes.toString(CryptoJS.enc.Utf8);

console.log(plaintext);
'''
...
```



# <a name="apidoc.module.crypto-js.TripleDES"></a>[module crypto-js.TripleDES](#apidoc.module.crypto-js.TripleDES)

#### <a name="apidoc.element.crypto-js.TripleDES.decrypt"></a>[function <span class="apidocSignatureSpan">crypto-js.TripleDES.</span>decrypt (ciphertext, key, cfg)](#apidoc.element.crypto-js.TripleDES.decrypt)
- description and source-code
```javascript
decrypt = function (ciphertext, key, cfg) {
	                        return selectCipherStrategy(key).decrypt(cipher, ciphertext, key, cfg);
	                    }
```
- example usage
```shell
...
'''javascript
var CryptoJS = require("crypto-js");

// Encrypt
var ciphertext = CryptoJS.AES.encrypt('my message', 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var plaintext = bytes.toString(CryptoJS.enc.Utf8);

console.log(plaintext);
'''

#### Object encryption
...
```

#### <a name="apidoc.element.crypto-js.TripleDES.encrypt"></a>[function <span class="apidocSignatureSpan">crypto-js.TripleDES.</span>encrypt (message, key, cfg)](#apidoc.element.crypto-js.TripleDES.encrypt)
- description and source-code
```javascript
encrypt = function (message, key, cfg) {
	                        return selectCipherStrategy(key).encrypt(cipher, message, key, cfg);
	                    }
```
- example usage
```shell
...

#### Plain text encryption

'''javascript
var CryptoJS = require("crypto-js");

// Encrypt
var ciphertext = CryptoJS.AES.encrypt('my message', 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var plaintext = bytes.toString(CryptoJS.enc.Utf8);

console.log(plaintext);
'''
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
