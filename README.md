# api documentation for  [crypto-js (v3.1.8)](http://github.com/brix/crypto-js)  [![npm package](https://img.shields.io/npm/v/npmdoc-crypto-js.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-crypto-js) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-crypto-js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-crypto-js)
#### JavaScript library of crypto standards.

[![NPM](https://nodei.co/npm/crypto-js.png?downloads=true)](https://www.npmjs.com/package/crypto-js)

[![apidoc](https://npmdoc.github.io/node-npmdoc-crypto-js/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-crypto-js_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-crypto-js/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-crypto-js/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-crypto-js/build/screenCapture.npmPackageDependencyTree.svg)



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
1.  object <span class="apidocSignatureSpan">crypto-js.</span>crypto_js
1.  object <span class="apidocSignatureSpan">crypto-js.</span>enc
1.  object <span class="apidocSignatureSpan">crypto-js.</span>enc_base64
1.  object <span class="apidocSignatureSpan">crypto-js.</span>enc_hex
1.  object <span class="apidocSignatureSpan">crypto-js.</span>enc_latin1
1.  object <span class="apidocSignatureSpan">crypto-js.</span>enc_utf16
1.  object <span class="apidocSignatureSpan">crypto-js.</span>enc_utf8
1.  object <span class="apidocSignatureSpan">crypto-js.</span>format
1.  object <span class="apidocSignatureSpan">crypto-js.</span>format_hex
1.  object <span class="apidocSignatureSpan">crypto-js.</span>format_openssl
1.  object <span class="apidocSignatureSpan">crypto-js.</span>kdf
1.  object <span class="apidocSignatureSpan">crypto-js.</span>lib
1.  object <span class="apidocSignatureSpan">crypto-js.</span>lib_typedarrays
1.  object <span class="apidocSignatureSpan">crypto-js.</span>mode
1.  object <span class="apidocSignatureSpan">crypto-js.</span>mode_cfb
1.  object <span class="apidocSignatureSpan">crypto-js.</span>mode_ctr
1.  object <span class="apidocSignatureSpan">crypto-js.</span>mode_ctr_gladman
1.  object <span class="apidocSignatureSpan">crypto-js.</span>mode_ecb
1.  object <span class="apidocSignatureSpan">crypto-js.</span>mode_ofb
1.  object <span class="apidocSignatureSpan">crypto-js.</span>pad
1.  object <span class="apidocSignatureSpan">crypto-js.</span>pad_iso10126
1.  object <span class="apidocSignatureSpan">crypto-js.</span>pad_iso97971
1.  object <span class="apidocSignatureSpan">crypto-js.</span>pad_nopadding
1.  object <span class="apidocSignatureSpan">crypto-js.</span>pad_pkcs7
1.  object <span class="apidocSignatureSpan">crypto-js.</span>pad_zeropadding
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

#### [module crypto-js.crypto_js](#apidoc.module.crypto-js.crypto_js)
1.  [function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>EvpKDF (password, salt, cfg)](#apidoc.element.crypto-js.crypto_js.EvpKDF)
1.  [function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>HmacMD5 (message, key)](#apidoc.element.crypto-js.crypto_js.HmacMD5)
1.  [function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>HmacRIPEMD160 (message, key)](#apidoc.element.crypto-js.crypto_js.HmacRIPEMD160)
1.  [function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>HmacSHA1 (message, key)](#apidoc.element.crypto-js.crypto_js.HmacSHA1)
1.  [function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>HmacSHA224 (message, key)](#apidoc.element.crypto-js.crypto_js.HmacSHA224)
1.  [function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>HmacSHA256 (message, key)](#apidoc.element.crypto-js.crypto_js.HmacSHA256)
1.  [function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>HmacSHA3 (message, key)](#apidoc.element.crypto-js.crypto_js.HmacSHA3)
1.  [function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>HmacSHA384 (message, key)](#apidoc.element.crypto-js.crypto_js.HmacSHA384)
1.  [function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>HmacSHA512 (message, key)](#apidoc.element.crypto-js.crypto_js.HmacSHA512)
1.  [function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>MD5 (message, cfg)](#apidoc.element.crypto-js.crypto_js.MD5)
1.  [function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>PBKDF2 (password, salt, cfg)](#apidoc.element.crypto-js.crypto_js.PBKDF2)
1.  [function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>RIPEMD160 (message, cfg)](#apidoc.element.crypto-js.crypto_js.RIPEMD160)
1.  [function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>SHA1 (message, cfg)](#apidoc.element.crypto-js.crypto_js.SHA1)
1.  [function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>SHA224 (message, cfg)](#apidoc.element.crypto-js.crypto_js.SHA224)
1.  [function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>SHA256 (message, cfg)](#apidoc.element.crypto-js.crypto_js.SHA256)
1.  [function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>SHA3 (message, cfg)](#apidoc.element.crypto-js.crypto_js.SHA3)
1.  [function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>SHA384 (message, cfg)](#apidoc.element.crypto-js.crypto_js.SHA384)
1.  [function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>SHA512 (message, cfg)](#apidoc.element.crypto-js.crypto_js.SHA512)
1.  object <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>AES
1.  object <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>DES
1.  object <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>RC4
1.  object <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>RC4Drop
1.  object <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>Rabbit
1.  object <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>RabbitLegacy
1.  object <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>TripleDES
1.  object <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>algo
1.  object <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>enc
1.  object <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>format
1.  object <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>kdf
1.  object <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>lib
1.  object <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>mode
1.  object <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>pad
1.  object <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>x64

#### [module crypto-js.enc_base64](#apidoc.module.crypto-js.enc_base64)
1.  [function <span class="apidocSignatureSpan">crypto-js.enc_base64.</span>parse (base64Str)](#apidoc.element.crypto-js.enc_base64.parse)
1.  [function <span class="apidocSignatureSpan">crypto-js.enc_base64.</span>stringify (wordArray)](#apidoc.element.crypto-js.enc_base64.stringify)
1.  string <span class="apidocSignatureSpan">crypto-js.enc_base64.</span>_map

#### [module crypto-js.enc_hex](#apidoc.module.crypto-js.enc_hex)
1.  [function <span class="apidocSignatureSpan">crypto-js.enc_hex.</span>parse (hexStr)](#apidoc.element.crypto-js.enc_hex.parse)
1.  [function <span class="apidocSignatureSpan">crypto-js.enc_hex.</span>stringify (wordArray)](#apidoc.element.crypto-js.enc_hex.stringify)

#### [module crypto-js.enc_latin1](#apidoc.module.crypto-js.enc_latin1)
1.  [function <span class="apidocSignatureSpan">crypto-js.enc_latin1.</span>parse (latin1Str)](#apidoc.element.crypto-js.enc_latin1.parse)
1.  [function <span class="apidocSignatureSpan">crypto-js.enc_latin1.</span>stringify (wordArray)](#apidoc.element.crypto-js.enc_latin1.stringify)

#### [module crypto-js.enc_utf16](#apidoc.module.crypto-js.enc_utf16)
1.  [function <span class="apidocSignatureSpan">crypto-js.enc_utf16.</span>parse (utf16Str)](#apidoc.element.crypto-js.enc_utf16.parse)
1.  [function <span class="apidocSignatureSpan">crypto-js.enc_utf16.</span>stringify (wordArray)](#apidoc.element.crypto-js.enc_utf16.stringify)

#### [module crypto-js.enc_utf8](#apidoc.module.crypto-js.enc_utf8)
1.  [function <span class="apidocSignatureSpan">crypto-js.enc_utf8.</span>parse (utf8Str)](#apidoc.element.crypto-js.enc_utf8.parse)
1.  [function <span class="apidocSignatureSpan">crypto-js.enc_utf8.</span>stringify (wordArray)](#apidoc.element.crypto-js.enc_utf8.stringify)

#### [module crypto-js.format_hex](#apidoc.module.crypto-js.format_hex)
1.  [function <span class="apidocSignatureSpan">crypto-js.format_hex.</span>parse (input)](#apidoc.element.crypto-js.format_hex.parse)
1.  [function <span class="apidocSignatureSpan">crypto-js.format_hex.</span>stringify (cipherParams)](#apidoc.element.crypto-js.format_hex.stringify)

#### [module crypto-js.format_openssl](#apidoc.module.crypto-js.format_openssl)
1.  [function <span class="apidocSignatureSpan">crypto-js.format_openssl.</span>parse (openSSLStr)](#apidoc.element.crypto-js.format_openssl.parse)
1.  [function <span class="apidocSignatureSpan">crypto-js.format_openssl.</span>stringify (cipherParams)](#apidoc.element.crypto-js.format_openssl.stringify)

#### [module crypto-js.lib_typedarrays](#apidoc.module.crypto-js.lib_typedarrays)
1.  [function <span class="apidocSignatureSpan">crypto-js.lib_typedarrays.</span>clamp ()](#apidoc.element.crypto-js.lib_typedarrays.clamp)
1.  [function <span class="apidocSignatureSpan">crypto-js.lib_typedarrays.</span>clone ()](#apidoc.element.crypto-js.lib_typedarrays.clone)
1.  [function <span class="apidocSignatureSpan">crypto-js.lib_typedarrays.</span>concat (wordArray)](#apidoc.element.crypto-js.lib_typedarrays.concat)
1.  [function <span class="apidocSignatureSpan">crypto-js.lib_typedarrays.</span>init (typedArray)](#apidoc.element.crypto-js.lib_typedarrays.init)
1.  [function <span class="apidocSignatureSpan">crypto-js.lib_typedarrays.</span>random (nBytes)](#apidoc.element.crypto-js.lib_typedarrays.random)
1.  [function <span class="apidocSignatureSpan">crypto-js.lib_typedarrays.</span>toString (encoder)](#apidoc.element.crypto-js.lib_typedarrays.toString)

#### [module crypto-js.mode_cfb](#apidoc.module.crypto-js.mode_cfb)
1.  [function <span class="apidocSignatureSpan">crypto-js.mode_cfb.</span>init ()](#apidoc.element.crypto-js.mode_cfb.init)
1.  object <span class="apidocSignatureSpan">crypto-js.mode_cfb.</span>Decryptor
1.  object <span class="apidocSignatureSpan">crypto-js.mode_cfb.</span>Encryptor

#### [module crypto-js.mode_ctr](#apidoc.module.crypto-js.mode_ctr)
1.  [function <span class="apidocSignatureSpan">crypto-js.mode_ctr.</span>init ()](#apidoc.element.crypto-js.mode_ctr.init)
1.  object <span class="apidocSignatureSpan">crypto-js.mode_ctr.</span>Decryptor
1.  object <span class="apidocSignatureSpan">crypto-js.mode_ctr.</span>Encryptor

#### [module crypto-js.mode_ctr_gladman](#apidoc.module.crypto-js.mode_ctr_gladman)
1.  [function <span class="apidocSignatureSpan">crypto-js.mode_ctr_gladman.</span>init ()](#apidoc.element.crypto-js.mode_ctr_gladman.init)
1.  object <span class="apidocSignatureSpan">crypto-js.mode_ctr_gladman.</span>Decryptor
1.  object <span class="apidocSignatureSpan">crypto-js.mode_ctr_gladman.</span>Encryptor

#### [module crypto-js.mode_ecb](#apidoc.module.crypto-js.mode_ecb)
1.  [function <span class="apidocSignatureSpan">crypto-js.mode_ecb.</span>init ()](#apidoc.element.crypto-js.mode_ecb.init)
1.  object <span class="apidocSignatureSpan">crypto-js.mode_ecb.</span>Decryptor
1.  object <span class="apidocSignatureSpan">crypto-js.mode_ecb.</span>Encryptor

#### [module crypto-js.mode_ofb](#apidoc.module.crypto-js.mode_ofb)
1.  [function <span class="apidocSignatureSpan">crypto-js.mode_ofb.</span>init ()](#apidoc.element.crypto-js.mode_ofb.init)
1.  object <span class="apidocSignatureSpan">crypto-js.mode_ofb.</span>Decryptor
1.  object <span class="apidocSignatureSpan">crypto-js.mode_ofb.</span>Encryptor

#### [module crypto-js.pad_iso10126](#apidoc.module.crypto-js.pad_iso10126)
1.  [function <span class="apidocSignatureSpan">crypto-js.pad_iso10126.</span>pad (data, blockSize)](#apidoc.element.crypto-js.pad_iso10126.pad)
1.  [function <span class="apidocSignatureSpan">crypto-js.pad_iso10126.</span>unpad (data)](#apidoc.element.crypto-js.pad_iso10126.unpad)

#### [module crypto-js.pad_iso97971](#apidoc.module.crypto-js.pad_iso97971)
1.  [function <span class="apidocSignatureSpan">crypto-js.pad_iso97971.</span>pad (data, blockSize)](#apidoc.element.crypto-js.pad_iso97971.pad)
1.  [function <span class="apidocSignatureSpan">crypto-js.pad_iso97971.</span>unpad (data)](#apidoc.element.crypto-js.pad_iso97971.unpad)

#### [module crypto-js.pad_nopadding](#apidoc.module.crypto-js.pad_nopadding)
1.  [function <span class="apidocSignatureSpan">crypto-js.pad_nopadding.</span>pad ()](#apidoc.element.crypto-js.pad_nopadding.pad)
1.  [function <span class="apidocSignatureSpan">crypto-js.pad_nopadding.</span>unpad ()](#apidoc.element.crypto-js.pad_nopadding.unpad)

#### [module crypto-js.pad_pkcs7](#apidoc.module.crypto-js.pad_pkcs7)
1.  [function <span class="apidocSignatureSpan">crypto-js.pad_pkcs7.</span>pad (data, blockSize)](#apidoc.element.crypto-js.pad_pkcs7.pad)
1.  [function <span class="apidocSignatureSpan">crypto-js.pad_pkcs7.</span>unpad (data)](#apidoc.element.crypto-js.pad_pkcs7.unpad)

#### [module crypto-js.pad_zeropadding](#apidoc.module.crypto-js.pad_zeropadding)
1.  [function <span class="apidocSignatureSpan">crypto-js.pad_zeropadding.</span>pad (data, blockSize)](#apidoc.element.crypto-js.pad_zeropadding.pad)
1.  [function <span class="apidocSignatureSpan">crypto-js.pad_zeropadding.</span>unpad (data)](#apidoc.element.crypto-js.pad_zeropadding.unpad)



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
...
	     *
	     * @return {WordArray} The derived key.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var key = CryptoJS.EvpKDF(password, salt);
	     *     var key = CryptoJS.EvpKDF(password, salt, { keySize: 8 });
	     *     var key = CryptoJS.EvpKDF(password, salt, { keySize: 8, iterations: 1000 });
	     */
	    C.EvpKDF = function (password, salt, cfg) {
	        return EvpKDF.create(cfg).compute(password, salt);
	    };
	}());
...
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
...
	     *
	     * @return {WordArray} The HMAC.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hmac = CryptoJS.HmacMD5(message, key);
	     */
	    C.HmacMD5 = Hasher._createHmacHelper(MD5);
	}(Math));


	(function () {
	    // Shortcuts
...
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
...
	     *
	     * @return {WordArray} The HMAC.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hmac = CryptoJS.HmacRIPEMD160(message, key);
	     */
	    C.HmacRIPEMD160 = Hasher._createHmacHelper(RIPEMD160);
	}(Math));


	(function () {
	    // Shortcuts
...
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
...
	     *
	     * @return {WordArray} The HMAC.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hmac = CryptoJS.HmacSHA224(message, key);
	     */
	    C.HmacSHA224 = SHA256._createHmacHelper(SHA224);
	}());


	(function (undefined) {
	    // Shortcuts
...
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
...
	     *
	     * @return {WordArray} The HMAC.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hmac = CryptoJS.HmacSHA256(message, key);
	     */
	    C.HmacSHA256 = Hasher._createHmacHelper(SHA256);
	}(Math));


	(function () {
	    // Shortcuts
...
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
...
	     *
	     * @return {WordArray} The HMAC.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hmac = CryptoJS.HmacSHA3(message, key);
	     */
	    C.HmacSHA3 = Hasher._createHmacHelper(SHA3);
	}(Math));


	(function () {
	    // Shortcuts
...
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
...
	     *
	     * @return {WordArray} The HMAC.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hmac = CryptoJS.HmacSHA384(message, key);
	     */
	    C.HmacSHA384 = SHA512._createHmacHelper(SHA384);
	}());


	/**
	 * Cipher core components.
...
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
...
	     *
	     * @return {WordArray} The HMAC.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hmac = CryptoJS.HmacSHA512(message, key);
	     */
	    C.HmacSHA512 = Hasher._createHmacHelper(SHA512);
	}());


	(function () {
	    // Shortcuts
...
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
...
	     *
	     * @return {WordArray} The hash.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hash = CryptoJS.MD5('message');
	     *     var hash = CryptoJS.MD5(wordArray);
	     */
	    C.MD5 = Hasher._createHelper(MD5);

	    /**
	     * Shortcut function to the HMAC's object interface.
	     *
...
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
...
	     *
	     * @return {WordArray} The derived key.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var key = CryptoJS.PBKDF2(password, salt);
	     *     var key = CryptoJS.PBKDF2(password, salt, { keySize: 8 });
	     *     var key = CryptoJS.PBKDF2(password, salt, { keySize: 8, iterations: 1000 });
	     */
	    C.PBKDF2 = function (password, salt, cfg) {
	        return PBKDF2.create(cfg).compute(password, salt);
	    };
	}());
...
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
...
	     *
	     * @return {WordArray} The hash.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hash = CryptoJS.RIPEMD160('message');
	     *     var hash = CryptoJS.RIPEMD160(wordArray);
	     */
	    C.RIPEMD160 = Hasher._createHelper(RIPEMD160);

	    /**
	     * Shortcut function to the HMAC's object interface.
	     *
...
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
...
	     *
	     * @return {WordArray} The hash.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hash = CryptoJS.SHA1('message');
	     *     var hash = CryptoJS.SHA1(wordArray);
	     */
	    C.SHA1 = Hasher._createHelper(SHA1);

	    /**
	     * Shortcut function to the HMAC's object interface.
	     *
...
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
...
	     *
	     * @return {WordArray} The hash.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hash = CryptoJS.SHA224('message');
	     *     var hash = CryptoJS.SHA224(wordArray);
	     */
	    C.SHA224 = SHA256._createHelper(SHA224);

	    /**
	     * Shortcut function to the HMAC's object interface.
	     *
...
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
...
	     *
	     * @return {WordArray} The hash.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hash = CryptoJS.SHA3('message');
	     *     var hash = CryptoJS.SHA3(wordArray);
	     */
	    C.SHA3 = Hasher._createHelper(SHA3);

	    /**
	     * Shortcut function to the HMAC's object interface.
	     *
...
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
...
	     *
	     * @return {WordArray} The hash.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hash = CryptoJS.SHA384('message');
	     *     var hash = CryptoJS.SHA384(wordArray);
	     */
	    C.SHA384 = SHA512._createHelper(SHA384);

	    /**
	     * Shortcut function to the HMAC's object interface.
	     *
...
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
...
	     *
	     * @return {WordArray} The hash.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hash = CryptoJS.SHA512('message');
	     *     var hash = CryptoJS.SHA512(wordArray);
	     */
	    C.SHA512 = Hasher._createHelper(SHA512);

	    /**
	     * Shortcut function to the HMAC's object interface.
	     *
...
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



# <a name="apidoc.module.crypto-js.crypto_js"></a>[module crypto-js.crypto_js](#apidoc.module.crypto-js.crypto_js)

#### <a name="apidoc.element.crypto-js.crypto_js.EvpKDF"></a>[function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>EvpKDF (password, salt, cfg)](#apidoc.element.crypto-js.crypto_js.EvpKDF)
- description and source-code
```javascript
EvpKDF = function (password, salt, cfg) {
	        return EvpKDF.create(cfg).compute(password, salt);
	    }
```
- example usage
```shell
...
	     *
	     * @return {WordArray} The derived key.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var key = CryptoJS.EvpKDF(password, salt);
	     *     var key = CryptoJS.EvpKDF(password, salt, { keySize: 8 });
	     *     var key = CryptoJS.EvpKDF(password, salt, { keySize: 8, iterations: 1000 });
	     */
	    C.EvpKDF = function (password, salt, cfg) {
	        return EvpKDF.create(cfg).compute(password, salt);
	    };
	}());
...
```

#### <a name="apidoc.element.crypto-js.crypto_js.HmacMD5"></a>[function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>HmacMD5 (message, key)](#apidoc.element.crypto-js.crypto_js.HmacMD5)
- description and source-code
```javascript
HmacMD5 = function (message, key) {
	                return new C_algo.HMAC.init(hasher, key).finalize(message);
	            }
```
- example usage
```shell
...
	     *
	     * @return {WordArray} The HMAC.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hmac = CryptoJS.HmacMD5(message, key);
	     */
	    C.HmacMD5 = Hasher._createHmacHelper(MD5);
	}(Math));


	(function () {
	    // Shortcuts
...
```

#### <a name="apidoc.element.crypto-js.crypto_js.HmacRIPEMD160"></a>[function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>HmacRIPEMD160 (message, key)](#apidoc.element.crypto-js.crypto_js.HmacRIPEMD160)
- description and source-code
```javascript
HmacRIPEMD160 = function (message, key) {
	                return new C_algo.HMAC.init(hasher, key).finalize(message);
	            }
```
- example usage
```shell
...
	     *
	     * @return {WordArray} The HMAC.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hmac = CryptoJS.HmacRIPEMD160(message, key);
	     */
	    C.HmacRIPEMD160 = Hasher._createHmacHelper(RIPEMD160);
	}(Math));


	(function () {
	    // Shortcuts
...
```

#### <a name="apidoc.element.crypto-js.crypto_js.HmacSHA1"></a>[function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>HmacSHA1 (message, key)](#apidoc.element.crypto-js.crypto_js.HmacSHA1)
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

#### <a name="apidoc.element.crypto-js.crypto_js.HmacSHA224"></a>[function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>HmacSHA224 (message, key)](#apidoc.element.crypto-js.crypto_js.HmacSHA224)
- description and source-code
```javascript
HmacSHA224 = function (message, key) {
	                return new C_algo.HMAC.init(hasher, key).finalize(message);
	            }
```
- example usage
```shell
...
	     *
	     * @return {WordArray} The HMAC.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hmac = CryptoJS.HmacSHA224(message, key);
	     */
	    C.HmacSHA224 = SHA256._createHmacHelper(SHA224);
	}());


	(function (undefined) {
	    // Shortcuts
...
```

#### <a name="apidoc.element.crypto-js.crypto_js.HmacSHA256"></a>[function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>HmacSHA256 (message, key)](#apidoc.element.crypto-js.crypto_js.HmacSHA256)
- description and source-code
```javascript
HmacSHA256 = function (message, key) {
	                return new C_algo.HMAC.init(hasher, key).finalize(message);
	            }
```
- example usage
```shell
...
	     *
	     * @return {WordArray} The HMAC.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hmac = CryptoJS.HmacSHA256(message, key);
	     */
	    C.HmacSHA256 = Hasher._createHmacHelper(SHA256);
	}(Math));


	(function () {
	    // Shortcuts
...
```

#### <a name="apidoc.element.crypto-js.crypto_js.HmacSHA3"></a>[function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>HmacSHA3 (message, key)](#apidoc.element.crypto-js.crypto_js.HmacSHA3)
- description and source-code
```javascript
HmacSHA3 = function (message, key) {
	                return new C_algo.HMAC.init(hasher, key).finalize(message);
	            }
```
- example usage
```shell
...
	     *
	     * @return {WordArray} The HMAC.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hmac = CryptoJS.HmacSHA3(message, key);
	     */
	    C.HmacSHA3 = Hasher._createHmacHelper(SHA3);
	}(Math));


	(function () {
	    // Shortcuts
...
```

#### <a name="apidoc.element.crypto-js.crypto_js.HmacSHA384"></a>[function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>HmacSHA384 (message, key)](#apidoc.element.crypto-js.crypto_js.HmacSHA384)
- description and source-code
```javascript
HmacSHA384 = function (message, key) {
	                return new C_algo.HMAC.init(hasher, key).finalize(message);
	            }
```
- example usage
```shell
...
	     *
	     * @return {WordArray} The HMAC.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hmac = CryptoJS.HmacSHA384(message, key);
	     */
	    C.HmacSHA384 = SHA512._createHmacHelper(SHA384);
	}());


	/**
	 * Cipher core components.
...
```

#### <a name="apidoc.element.crypto-js.crypto_js.HmacSHA512"></a>[function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>HmacSHA512 (message, key)](#apidoc.element.crypto-js.crypto_js.HmacSHA512)
- description and source-code
```javascript
HmacSHA512 = function (message, key) {
	                return new C_algo.HMAC.init(hasher, key).finalize(message);
	            }
```
- example usage
```shell
...
	     *
	     * @return {WordArray} The HMAC.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hmac = CryptoJS.HmacSHA512(message, key);
	     */
	    C.HmacSHA512 = Hasher._createHmacHelper(SHA512);
	}());


	(function () {
	    // Shortcuts
...
```

#### <a name="apidoc.element.crypto-js.crypto_js.MD5"></a>[function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>MD5 (message, cfg)](#apidoc.element.crypto-js.crypto_js.MD5)
- description and source-code
```javascript
MD5 = function (message, cfg) {
	                return new hasher.init(cfg).finalize(message);
	            }
```
- example usage
```shell
...
	     *
	     * @return {WordArray} The hash.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hash = CryptoJS.MD5('message');
	     *     var hash = CryptoJS.MD5(wordArray);
	     */
	    C.MD5 = Hasher._createHelper(MD5);

	    /**
	     * Shortcut function to the HMAC's object interface.
	     *
...
```

#### <a name="apidoc.element.crypto-js.crypto_js.PBKDF2"></a>[function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>PBKDF2 (password, salt, cfg)](#apidoc.element.crypto-js.crypto_js.PBKDF2)
- description and source-code
```javascript
PBKDF2 = function (password, salt, cfg) {
	        return PBKDF2.create(cfg).compute(password, salt);
	    }
```
- example usage
```shell
...
	     *
	     * @return {WordArray} The derived key.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var key = CryptoJS.PBKDF2(password, salt);
	     *     var key = CryptoJS.PBKDF2(password, salt, { keySize: 8 });
	     *     var key = CryptoJS.PBKDF2(password, salt, { keySize: 8, iterations: 1000 });
	     */
	    C.PBKDF2 = function (password, salt, cfg) {
	        return PBKDF2.create(cfg).compute(password, salt);
	    };
	}());
...
```

#### <a name="apidoc.element.crypto-js.crypto_js.RIPEMD160"></a>[function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>RIPEMD160 (message, cfg)](#apidoc.element.crypto-js.crypto_js.RIPEMD160)
- description and source-code
```javascript
RIPEMD160 = function (message, cfg) {
	                return new hasher.init(cfg).finalize(message);
	            }
```
- example usage
```shell
...
	     *
	     * @return {WordArray} The hash.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hash = CryptoJS.RIPEMD160('message');
	     *     var hash = CryptoJS.RIPEMD160(wordArray);
	     */
	    C.RIPEMD160 = Hasher._createHelper(RIPEMD160);

	    /**
	     * Shortcut function to the HMAC's object interface.
	     *
...
```

#### <a name="apidoc.element.crypto-js.crypto_js.SHA1"></a>[function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>SHA1 (message, cfg)](#apidoc.element.crypto-js.crypto_js.SHA1)
- description and source-code
```javascript
SHA1 = function (message, cfg) {
	                return new hasher.init(cfg).finalize(message);
	            }
```
- example usage
```shell
...
	     *
	     * @return {WordArray} The hash.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hash = CryptoJS.SHA1('message');
	     *     var hash = CryptoJS.SHA1(wordArray);
	     */
	    C.SHA1 = Hasher._createHelper(SHA1);

	    /**
	     * Shortcut function to the HMAC's object interface.
	     *
...
```

#### <a name="apidoc.element.crypto-js.crypto_js.SHA224"></a>[function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>SHA224 (message, cfg)](#apidoc.element.crypto-js.crypto_js.SHA224)
- description and source-code
```javascript
SHA224 = function (message, cfg) {
	                return new hasher.init(cfg).finalize(message);
	            }
```
- example usage
```shell
...
	     *
	     * @return {WordArray} The hash.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hash = CryptoJS.SHA224('message');
	     *     var hash = CryptoJS.SHA224(wordArray);
	     */
	    C.SHA224 = SHA256._createHelper(SHA224);

	    /**
	     * Shortcut function to the HMAC's object interface.
	     *
...
```

#### <a name="apidoc.element.crypto-js.crypto_js.SHA256"></a>[function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>SHA256 (message, cfg)](#apidoc.element.crypto-js.crypto_js.SHA256)
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

#### <a name="apidoc.element.crypto-js.crypto_js.SHA3"></a>[function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>SHA3 (message, cfg)](#apidoc.element.crypto-js.crypto_js.SHA3)
- description and source-code
```javascript
SHA3 = function (message, cfg) {
	                return new hasher.init(cfg).finalize(message);
	            }
```
- example usage
```shell
...
	     *
	     * @return {WordArray} The hash.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hash = CryptoJS.SHA3('message');
	     *     var hash = CryptoJS.SHA3(wordArray);
	     */
	    C.SHA3 = Hasher._createHelper(SHA3);

	    /**
	     * Shortcut function to the HMAC's object interface.
	     *
...
```

#### <a name="apidoc.element.crypto-js.crypto_js.SHA384"></a>[function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>SHA384 (message, cfg)](#apidoc.element.crypto-js.crypto_js.SHA384)
- description and source-code
```javascript
SHA384 = function (message, cfg) {
	                return new hasher.init(cfg).finalize(message);
	            }
```
- example usage
```shell
...
	     *
	     * @return {WordArray} The hash.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hash = CryptoJS.SHA384('message');
	     *     var hash = CryptoJS.SHA384(wordArray);
	     */
	    C.SHA384 = SHA512._createHelper(SHA384);

	    /**
	     * Shortcut function to the HMAC's object interface.
	     *
...
```

#### <a name="apidoc.element.crypto-js.crypto_js.SHA512"></a>[function <span class="apidocSignatureSpan">crypto-js.crypto_js.</span>SHA512 (message, cfg)](#apidoc.element.crypto-js.crypto_js.SHA512)
- description and source-code
```javascript
SHA512 = function (message, cfg) {
	                return new hasher.init(cfg).finalize(message);
	            }
```
- example usage
```shell
...
	     *
	     * @return {WordArray} The hash.
	     *
	     * @static
	     *
	     * @example
	     *
	     *     var hash = CryptoJS.SHA512('message');
	     *     var hash = CryptoJS.SHA512(wordArray);
	     */
	    C.SHA512 = Hasher._createHelper(SHA512);

	    /**
	     * Shortcut function to the HMAC's object interface.
	     *
...
```



# <a name="apidoc.module.crypto-js.enc_base64"></a>[module crypto-js.enc_base64](#apidoc.module.crypto-js.enc_base64)

#### <a name="apidoc.element.crypto-js.enc_base64.parse"></a>[function <span class="apidocSignatureSpan">crypto-js.enc_base64.</span>parse (base64Str)](#apidoc.element.crypto-js.enc_base64.parse)
- description and source-code
```javascript
parse = function (base64Str) {
	            // Shortcuts
	            var base64StrLength = base64Str.length;
	            var map = this._map;
	            var reverseMap = this._reverseMap;

	            if (!reverseMap) {
	                    reverseMap = this._reverseMap = [];
	                    for (var j = 0; j < map.length; j++) {
	                        reverseMap[map.charCodeAt(j)] = j;
	                    }
	            }

	            // Ignore padding
	            var paddingChar = map.charAt(64);
	            if (paddingChar) {
	                var paddingIndex = base64Str.indexOf(paddingChar);
	                if (paddingIndex !== -1) {
	                    base64StrLength = paddingIndex;
	                }
	            }

	            // Convert
	            return parseLoop(base64Str, base64StrLength, reverseMap);

	        }
```
- example usage
```shell
...
var data = [{id: 1}, {id: 2}]

// Encrypt
var ciphertext = CryptoJS.AES.encrypt(JSON.stringify(data), 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var decryptedData = JSON.parse(bytes.toString(CryptoJS.enc.Utf8));

console.log(decryptedData);
'''

### List of modules
...
```

#### <a name="apidoc.element.crypto-js.enc_base64.stringify"></a>[function <span class="apidocSignatureSpan">crypto-js.enc_base64.</span>stringify (wordArray)](#apidoc.element.crypto-js.enc_base64.stringify)
- description and source-code
```javascript
stringify = function (wordArray) {
	            // Shortcuts
	            var words = wordArray.words;
	            var sigBytes = wordArray.sigBytes;
	            var map = this._map;

	            // Clamp excess bits
	            wordArray.clamp();

	            // Convert
	            var base64Chars = [];
	            for (var i = 0; i < sigBytes; i += 3) {
	                var byte1 = (words[i >>> 2]       >>> (24 - (i % 4) * 8))       & 0xff;
	                var byte2 = (words[(i + 1) >>> 2] >>> (24 - ((i + 1) % 4) * 8)) & 0xff;
	                var byte3 = (words[(i + 2) >>> 2] >>> (24 - ((i + 2) % 4) * 8)) & 0xff;

	                var triplet = (byte1 << 16) | (byte2 << 8) | byte3;

	                for (var j = 0; (j < 4) && (i + j * 0.75 < sigBytes); j++) {
	                    base64Chars.push(map.charAt((triplet >>> (6 * (3 - j))) & 0x3f));
	                }
	            }

	            // Add padding
	            var paddingChar = map.charAt(64);
	            if (paddingChar) {
	                while (base64Chars.length % 4) {
	                    base64Chars.push(paddingChar);
	                }
	            }

	            return base64Chars.join('');
	        }
```
- example usage
```shell
...

'''javascript
var CryptoJS = require("crypto-js");

var data = [{id: 1}, {id: 2}]

// Encrypt
var ciphertext = CryptoJS.AES.encrypt(JSON.stringify(data), 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var decryptedData = JSON.parse(bytes.toString(CryptoJS.enc.Utf8));

console.log(decryptedData);
'''
...
```



# <a name="apidoc.module.crypto-js.enc_hex"></a>[module crypto-js.enc_hex](#apidoc.module.crypto-js.enc_hex)

#### <a name="apidoc.element.crypto-js.enc_hex.parse"></a>[function <span class="apidocSignatureSpan">crypto-js.enc_hex.</span>parse (hexStr)](#apidoc.element.crypto-js.enc_hex.parse)
- description and source-code
```javascript
parse = function (hexStr) {
	            // Shortcut
	            var hexStrLength = hexStr.length;

	            // Convert
	            var words = [];
	            for (var i = 0; i < hexStrLength; i += 2) {
	                words[i >>> 3] |= parseInt(hexStr.substr(i, 2), 16) << (24 - (i % 8) * 4);
	            }

	            return new WordArray.init(words, hexStrLength / 2);
	        }
```
- example usage
```shell
...
var data = [{id: 1}, {id: 2}]

// Encrypt
var ciphertext = CryptoJS.AES.encrypt(JSON.stringify(data), 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var decryptedData = JSON.parse(bytes.toString(CryptoJS.enc.Utf8));

console.log(decryptedData);
'''

### List of modules
...
```

#### <a name="apidoc.element.crypto-js.enc_hex.stringify"></a>[function <span class="apidocSignatureSpan">crypto-js.enc_hex.</span>stringify (wordArray)](#apidoc.element.crypto-js.enc_hex.stringify)
- description and source-code
```javascript
stringify = function (wordArray) {
	            // Shortcuts
	            var words = wordArray.words;
	            var sigBytes = wordArray.sigBytes;

	            // Convert
	            var hexChars = [];
	            for (var i = 0; i < sigBytes; i++) {
	                var bite = (words[i >>> 2] >>> (24 - (i % 4) * 8)) & 0xff;
	                hexChars.push((bite >>> 4).toString(16));
	                hexChars.push((bite & 0x0f).toString(16));
	            }

	            return hexChars.join('');
	        }
```
- example usage
```shell
...

'''javascript
var CryptoJS = require("crypto-js");

var data = [{id: 1}, {id: 2}]

// Encrypt
var ciphertext = CryptoJS.AES.encrypt(JSON.stringify(data), 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var decryptedData = JSON.parse(bytes.toString(CryptoJS.enc.Utf8));

console.log(decryptedData);
'''
...
```



# <a name="apidoc.module.crypto-js.enc_latin1"></a>[module crypto-js.enc_latin1](#apidoc.module.crypto-js.enc_latin1)

#### <a name="apidoc.element.crypto-js.enc_latin1.parse"></a>[function <span class="apidocSignatureSpan">crypto-js.enc_latin1.</span>parse (latin1Str)](#apidoc.element.crypto-js.enc_latin1.parse)
- description and source-code
```javascript
parse = function (latin1Str) {
	            // Shortcut
	            var latin1StrLength = latin1Str.length;

	            // Convert
	            var words = [];
	            for (var i = 0; i < latin1StrLength; i++) {
	                words[i >>> 2] |= (latin1Str.charCodeAt(i) & 0xff) << (24 - (i % 4) * 8);
	            }

	            return new WordArray.init(words, latin1StrLength);
	        }
```
- example usage
```shell
...
var data = [{id: 1}, {id: 2}]

// Encrypt
var ciphertext = CryptoJS.AES.encrypt(JSON.stringify(data), 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var decryptedData = JSON.parse(bytes.toString(CryptoJS.enc.Utf8));

console.log(decryptedData);
'''

### List of modules
...
```

#### <a name="apidoc.element.crypto-js.enc_latin1.stringify"></a>[function <span class="apidocSignatureSpan">crypto-js.enc_latin1.</span>stringify (wordArray)](#apidoc.element.crypto-js.enc_latin1.stringify)
- description and source-code
```javascript
stringify = function (wordArray) {
	            // Shortcuts
	            var words = wordArray.words;
	            var sigBytes = wordArray.sigBytes;

	            // Convert
	            var latin1Chars = [];
	            for (var i = 0; i < sigBytes; i++) {
	                var bite = (words[i >>> 2] >>> (24 - (i % 4) * 8)) & 0xff;
	                latin1Chars.push(String.fromCharCode(bite));
	            }

	            return latin1Chars.join('');
	        }
```
- example usage
```shell
...

'''javascript
var CryptoJS = require("crypto-js");

var data = [{id: 1}, {id: 2}]

// Encrypt
var ciphertext = CryptoJS.AES.encrypt(JSON.stringify(data), 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var decryptedData = JSON.parse(bytes.toString(CryptoJS.enc.Utf8));

console.log(decryptedData);
'''
...
```



# <a name="apidoc.module.crypto-js.enc_utf16"></a>[module crypto-js.enc_utf16](#apidoc.module.crypto-js.enc_utf16)

#### <a name="apidoc.element.crypto-js.enc_utf16.parse"></a>[function <span class="apidocSignatureSpan">crypto-js.enc_utf16.</span>parse (utf16Str)](#apidoc.element.crypto-js.enc_utf16.parse)
- description and source-code
```javascript
parse = function (utf16Str) {
	            // Shortcut
	            var utf16StrLength = utf16Str.length;

	            // Convert
	            var words = [];
	            for (var i = 0; i < utf16StrLength; i++) {
	                words[i >>> 1] |= utf16Str.charCodeAt(i) << (16 - (i % 2) * 16);
	            }

	            return WordArray.create(words, utf16StrLength * 2);
	        }
```
- example usage
```shell
...
var data = [{id: 1}, {id: 2}]

// Encrypt
var ciphertext = CryptoJS.AES.encrypt(JSON.stringify(data), 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var decryptedData = JSON.parse(bytes.toString(CryptoJS.enc.Utf8));

console.log(decryptedData);
'''

### List of modules
...
```

#### <a name="apidoc.element.crypto-js.enc_utf16.stringify"></a>[function <span class="apidocSignatureSpan">crypto-js.enc_utf16.</span>stringify (wordArray)](#apidoc.element.crypto-js.enc_utf16.stringify)
- description and source-code
```javascript
stringify = function (wordArray) {
	            // Shortcuts
	            var words = wordArray.words;
	            var sigBytes = wordArray.sigBytes;

	            // Convert
	            var utf16Chars = [];
	            for (var i = 0; i < sigBytes; i += 2) {
	                var codePoint = (words[i >>> 2] >>> (16 - (i % 4) * 8)) & 0xffff;
	                utf16Chars.push(String.fromCharCode(codePoint));
	            }

	            return utf16Chars.join('');
	        }
```
- example usage
```shell
...

'''javascript
var CryptoJS = require("crypto-js");

var data = [{id: 1}, {id: 2}]

// Encrypt
var ciphertext = CryptoJS.AES.encrypt(JSON.stringify(data), 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var decryptedData = JSON.parse(bytes.toString(CryptoJS.enc.Utf8));

console.log(decryptedData);
'''
...
```



# <a name="apidoc.module.crypto-js.enc_utf8"></a>[module crypto-js.enc_utf8](#apidoc.module.crypto-js.enc_utf8)

#### <a name="apidoc.element.crypto-js.enc_utf8.parse"></a>[function <span class="apidocSignatureSpan">crypto-js.enc_utf8.</span>parse (utf8Str)](#apidoc.element.crypto-js.enc_utf8.parse)
- description and source-code
```javascript
parse = function (utf8Str) {
	            return Latin1.parse(unescape(encodeURIComponent(utf8Str)));
	        }
```
- example usage
```shell
...
var data = [{id: 1}, {id: 2}]

// Encrypt
var ciphertext = CryptoJS.AES.encrypt(JSON.stringify(data), 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var decryptedData = JSON.parse(bytes.toString(CryptoJS.enc.Utf8));

console.log(decryptedData);
'''

### List of modules
...
```

#### <a name="apidoc.element.crypto-js.enc_utf8.stringify"></a>[function <span class="apidocSignatureSpan">crypto-js.enc_utf8.</span>stringify (wordArray)](#apidoc.element.crypto-js.enc_utf8.stringify)
- description and source-code
```javascript
stringify = function (wordArray) {
	            try {
	                return decodeURIComponent(escape(Latin1.stringify(wordArray)));
	            } catch (e) {
	                throw new Error('Malformed UTF-8 data');
	            }
	        }
```
- example usage
```shell
...

'''javascript
var CryptoJS = require("crypto-js");

var data = [{id: 1}, {id: 2}]

// Encrypt
var ciphertext = CryptoJS.AES.encrypt(JSON.stringify(data), 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var decryptedData = JSON.parse(bytes.toString(CryptoJS.enc.Utf8));

console.log(decryptedData);
'''
...
```



# <a name="apidoc.module.crypto-js.format_hex"></a>[module crypto-js.format_hex](#apidoc.module.crypto-js.format_hex)

#### <a name="apidoc.element.crypto-js.format_hex.parse"></a>[function <span class="apidocSignatureSpan">crypto-js.format_hex.</span>parse (input)](#apidoc.element.crypto-js.format_hex.parse)
- description and source-code
```javascript
parse = function (input) {
	            var ciphertext = Hex.parse(input);
	            return CipherParams.create({ ciphertext: ciphertext });
	        }
```
- example usage
```shell
...
var data = [{id: 1}, {id: 2}]

// Encrypt
var ciphertext = CryptoJS.AES.encrypt(JSON.stringify(data), 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var decryptedData = JSON.parse(bytes.toString(CryptoJS.enc.Utf8));

console.log(decryptedData);
'''

### List of modules
...
```

#### <a name="apidoc.element.crypto-js.format_hex.stringify"></a>[function <span class="apidocSignatureSpan">crypto-js.format_hex.</span>stringify (cipherParams)](#apidoc.element.crypto-js.format_hex.stringify)
- description and source-code
```javascript
stringify = function (cipherParams) {
	            return cipherParams.ciphertext.toString(Hex);
	        }
```
- example usage
```shell
...

'''javascript
var CryptoJS = require("crypto-js");

var data = [{id: 1}, {id: 2}]

// Encrypt
var ciphertext = CryptoJS.AES.encrypt(JSON.stringify(data), 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var decryptedData = JSON.parse(bytes.toString(CryptoJS.enc.Utf8));

console.log(decryptedData);
'''
...
```



# <a name="apidoc.module.crypto-js.format_openssl"></a>[module crypto-js.format_openssl](#apidoc.module.crypto-js.format_openssl)

#### <a name="apidoc.element.crypto-js.format_openssl.parse"></a>[function <span class="apidocSignatureSpan">crypto-js.format_openssl.</span>parse (openSSLStr)](#apidoc.element.crypto-js.format_openssl.parse)
- description and source-code
```javascript
parse = function (openSSLStr) {
	            // Parse base64
	            var ciphertext = Base64.parse(openSSLStr);

	            // Shortcut
	            var ciphertextWords = ciphertext.words;

	            // Test for salt
	            if (ciphertextWords[0] == 0x53616c74 && ciphertextWords[1] == 0x65645f5f) {
	                // Extract salt
	                var salt = WordArray.create(ciphertextWords.slice(2, 4));

	                // Remove salt from ciphertext
	                ciphertextWords.splice(0, 4);
	                ciphertext.sigBytes -= 16;
	            }

	            return CipherParams.create({ ciphertext: ciphertext, salt: salt });
	        }
```
- example usage
```shell
...
var data = [{id: 1}, {id: 2}]

// Encrypt
var ciphertext = CryptoJS.AES.encrypt(JSON.stringify(data), 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var decryptedData = JSON.parse(bytes.toString(CryptoJS.enc.Utf8));

console.log(decryptedData);
'''

### List of modules
...
```

#### <a name="apidoc.element.crypto-js.format_openssl.stringify"></a>[function <span class="apidocSignatureSpan">crypto-js.format_openssl.</span>stringify (cipherParams)](#apidoc.element.crypto-js.format_openssl.stringify)
- description and source-code
```javascript
stringify = function (cipherParams) {
	            // Shortcuts
	            var ciphertext = cipherParams.ciphertext;
	            var salt = cipherParams.salt;

	            // Format
	            if (salt) {
	                var wordArray = WordArray.create([0x53616c74, 0x65645f5f]).concat(salt).concat(ciphertext);
	            } else {
	                var wordArray = ciphertext;
	            }

	            return wordArray.toString(Base64);
	        }
```
- example usage
```shell
...

'''javascript
var CryptoJS = require("crypto-js");

var data = [{id: 1}, {id: 2}]

// Encrypt
var ciphertext = CryptoJS.AES.encrypt(JSON.stringify(data), 'secret key 123');

// Decrypt
var bytes  = CryptoJS.AES.decrypt(ciphertext.toString(), 'secret key 123');
var decryptedData = JSON.parse(bytes.toString(CryptoJS.enc.Utf8));

console.log(decryptedData);
'''
...
```



# <a name="apidoc.module.crypto-js.lib_typedarrays"></a>[module crypto-js.lib_typedarrays](#apidoc.module.crypto-js.lib_typedarrays)

#### <a name="apidoc.element.crypto-js.lib_typedarrays.clamp"></a>[function <span class="apidocSignatureSpan">crypto-js.lib_typedarrays.</span>clamp ()](#apidoc.element.crypto-js.lib_typedarrays.clamp)
- description and source-code
```javascript
clamp = function () {
	            // Shortcuts
	            var words = this.words;
	            var sigBytes = this.sigBytes;

	            // Clamp
	            words[sigBytes >>> 2] &= 0xffffffff << (32 - (sigBytes % 4) * 8);
	            words.length = Math.ceil(sigBytes / 4);
	        }
```
- example usage
```shell
...
	            // Shortcuts
	            var thisWords = this.words;
	            var thatWords = wordArray.words;
	            var thisSigBytes = this.sigBytes;
	            var thatSigBytes = wordArray.sigBytes;

	            // Clamp excess bits
	            this.clamp();

	            // Concat
	            if (thisSigBytes % 4) {
	                // Copy one byte at a time
	                for (var i = 0; i < thatSigBytes; i++) {
	                    var thatByte = (thatWords[i >>> 2] >>> (24 - (i % 4) * 8)) & 0xff;
	                    thisWords[(thisSigBytes + i) >>> 2] |= thatByte << (24 - ((thisSigBytes + i) % 4) * 8);
...
```

#### <a name="apidoc.element.crypto-js.lib_typedarrays.clone"></a>[function <span class="apidocSignatureSpan">crypto-js.lib_typedarrays.</span>clone ()](#apidoc.element.crypto-js.lib_typedarrays.clone)
- description and source-code
```javascript
clone = function () {
	            var clone = Base.clone.call(this);
	            clone.words = this.words.slice(0);

	            return clone;
	        }
```
- example usage
```shell
...
	            /**
	             * Creates a copy of this object.
	             *
	             * @return {Object} The clone.
	             *
	             * @example
	             *
	             *     var clone = instance.clone();
	             */
	            clone: function () {
	                return this.init.prototype.extend(this);
	            }
	        };
	    }());
...
```

#### <a name="apidoc.element.crypto-js.lib_typedarrays.concat"></a>[function <span class="apidocSignatureSpan">crypto-js.lib_typedarrays.</span>concat (wordArray)](#apidoc.element.crypto-js.lib_typedarrays.concat)
- description and source-code
```javascript
concat = function (wordArray) {
	            // Shortcuts
	            var thisWords = this.words;
	            var thatWords = wordArray.words;
	            var thisSigBytes = this.sigBytes;
	            var thatSigBytes = wordArray.sigBytes;

	            // Clamp excess bits
	            this.clamp();

	            // Concat
	            if (thisSigBytes % 4) {
	                // Copy one byte at a time
	                for (var i = 0; i < thatSigBytes; i++) {
	                    var thatByte = (thatWords[i >>> 2] >>> (24 - (i % 4) * 8)) & 0xff;
	                    thisWords[(thisSigBytes + i) >>> 2] |= thatByte << (24 - ((thisSigBytes + i) % 4) * 8);
	                }
	            } else {
	                // Copy one word at a time
	                for (var i = 0; i < thatSigBytes; i += 4) {
	                    thisWords[(thisSigBytes + i) >>> 2] = thatWords[i >>> 2];
	                }
	            }
	            this.sigBytes += thatSigBytes;

	            // Chainable
	            return this;
	        }
```
- example usage
```shell
...
	         *
	         * @param {WordArray} wordArray The word array to append.
	         *
	         * @return {WordArray} This word array.
	         *
	         * @example
	         *
	         *     wordArray1.concat(wordArray2);
	         */
	        concat: function (wordArray) {
	            // Shortcuts
	            var thisWords = this.words;
	            var thatWords = wordArray.words;
	            var thisSigBytes = this.sigBytes;
	            var thatSigBytes = wordArray.sigBytes;
...
```

#### <a name="apidoc.element.crypto-js.lib_typedarrays.init"></a>[function <span class="apidocSignatureSpan">crypto-js.lib_typedarrays.</span>init (typedArray)](#apidoc.element.crypto-js.lib_typedarrays.init)
- description and source-code
```javascript
init = function (typedArray) {
	        // Convert buffers to uint8
	        if (typedArray instanceof ArrayBuffer) {
	            typedArray = new Uint8Array(typedArray);
	        }

	        // Convert other array views to uint8
	        if (
	            typedArray instanceof Int8Array ||
	            (typeof Uint8ClampedArray !== "undefined" && typedArray instanceof Uint8ClampedArray) ||
	            typedArray instanceof Int16Array ||
	            typedArray instanceof Uint16Array ||
	            typedArray instanceof Int32Array ||
	            typedArray instanceof Uint32Array ||
	            typedArray instanceof Float32Array ||
	            typedArray instanceof Float64Array
	        ) {
	            typedArray = new Uint8Array(typedArray.buffer, typedArray.byteOffset, typedArray.byteLength);
	        }

	        // Handle Uint8Array
	        if (typedArray instanceof Uint8Array) {
	            // Shortcut
	            var typedArrayByteLength = typedArray.byteLength;

	            // Extract bytes
	            var words = [];
	            for (var i = 0; i < typedArrayByteLength; i++) {
	                words[i >>> 2] |= typedArray[i] << (24 - (i % 4) * 8);
	            }

	            // Initialize this word array
	            superInit.call(this, words, typedArrayByteLength);
	        } else {
	            // Else call normal init
	            superInit.apply(this, arguments);
	        }
	    }
```
- example usage
```shell
...
	            for (var i = 0, rcache; i < nBytes; i += 4) {
	                var _r = r((rcache || Math.random()) * 0x100000000);

	                rcache = _r() * 0x3ade67b7;
	                words.push((_r() * 0x100000000) | 0);
	            }

	            return new WordArray.init(words, nBytes);
	        }
	    });

	    /**
	     * Encoder namespace.
	     */
	    var C_enc = C.enc = {};
...
```

#### <a name="apidoc.element.crypto-js.lib_typedarrays.random"></a>[function <span class="apidocSignatureSpan">crypto-js.lib_typedarrays.</span>random (nBytes)](#apidoc.element.crypto-js.lib_typedarrays.random)
- description and source-code
```javascript
random = function (nBytes) {
	            var words = [];

	            var r = (function (m_w) {
	                var m_w = m_w;
	                var m_z = 0x3ade68b1;
	                var mask = 0xffffffff;

	                return function () {
	                    m_z = (0x9069 * (m_z & 0xFFFF) + (m_z >> 0x10)) & mask;
	                    m_w = (0x4650 * (m_w & 0xFFFF) + (m_w >> 0x10)) & mask;
	                    var result = ((m_z << 0x10) + m_w) & mask;
	                    result /= 0x100000000;
	                    result += 0.5;
	                    return result * (Math.random() > .5 ? 1 : -1);
	                }
	            });

	            for (var i = 0, rcache; i < nBytes; i += 4) {
	                var _r = r((rcache || Math.random()) * 0x100000000);

	                rcache = _r() * 0x3ade67b7;
	                words.push((_r() * 0x100000000) | 0);
	            }

	            return new WordArray.init(words, nBytes);
	        }
```
- example usage
```shell
...
	         *
	         * @return {WordArray} The random word array.
	         *
	         * @static
	         *
	         * @example
	         *
	         *     var wordArray = CryptoJS.lib.WordArray.random(16);
	         */
	        random: function (nBytes) {
	            var words = [];

	            var r = (function (m_w) {
	                var m_w = m_w;
	                var m_z = 0x3ade68b1;
...
```

#### <a name="apidoc.element.crypto-js.lib_typedarrays.toString"></a>[function <span class="apidocSignatureSpan">crypto-js.lib_typedarrays.</span>toString (encoder)](#apidoc.element.crypto-js.lib_typedarrays.toString)
- description and source-code
```javascript
toString = function (encoder) {
	            return (encoder || Hex).stringify(this);
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



# <a name="apidoc.module.crypto-js.mode_cfb"></a>[module crypto-js.mode_cfb](#apidoc.module.crypto-js.mode_cfb)

#### <a name="apidoc.element.crypto-js.mode_cfb.init"></a>[function <span class="apidocSignatureSpan">crypto-js.mode_cfb.</span>init ()](#apidoc.element.crypto-js.mode_cfb.init)
- description and source-code
```javascript
init = function () {
	                        subtype.$super.init.apply(this, arguments);
	                    }
```
- example usage
```shell
...
	            for (var i = 0, rcache; i < nBytes; i += 4) {
	                var _r = r((rcache || Math.random()) * 0x100000000);

	                rcache = _r() * 0x3ade67b7;
	                words.push((_r() * 0x100000000) | 0);
	            }

	            return new WordArray.init(words, nBytes);
	        }
	    });

	    /**
	     * Encoder namespace.
	     */
	    var C_enc = C.enc = {};
...
```



# <a name="apidoc.module.crypto-js.mode_ctr"></a>[module crypto-js.mode_ctr](#apidoc.module.crypto-js.mode_ctr)

#### <a name="apidoc.element.crypto-js.mode_ctr.init"></a>[function <span class="apidocSignatureSpan">crypto-js.mode_ctr.</span>init ()](#apidoc.element.crypto-js.mode_ctr.init)
- description and source-code
```javascript
init = function () {
	                        subtype.$super.init.apply(this, arguments);
	                    }
```
- example usage
```shell
...
	            for (var i = 0, rcache; i < nBytes; i += 4) {
	                var _r = r((rcache || Math.random()) * 0x100000000);

	                rcache = _r() * 0x3ade67b7;
	                words.push((_r() * 0x100000000) | 0);
	            }

	            return new WordArray.init(words, nBytes);
	        }
	    });

	    /**
	     * Encoder namespace.
	     */
	    var C_enc = C.enc = {};
...
```



# <a name="apidoc.module.crypto-js.mode_ctr_gladman"></a>[module crypto-js.mode_ctr_gladman](#apidoc.module.crypto-js.mode_ctr_gladman)

#### <a name="apidoc.element.crypto-js.mode_ctr_gladman.init"></a>[function <span class="apidocSignatureSpan">crypto-js.mode_ctr_gladman.</span>init ()](#apidoc.element.crypto-js.mode_ctr_gladman.init)
- description and source-code
```javascript
init = function () {
	                        subtype.$super.init.apply(this, arguments);
	                    }
```
- example usage
```shell
...
	            for (var i = 0, rcache; i < nBytes; i += 4) {
	                var _r = r((rcache || Math.random()) * 0x100000000);

	                rcache = _r() * 0x3ade67b7;
	                words.push((_r() * 0x100000000) | 0);
	            }

	            return new WordArray.init(words, nBytes);
	        }
	    });

	    /**
	     * Encoder namespace.
	     */
	    var C_enc = C.enc = {};
...
```



# <a name="apidoc.module.crypto-js.mode_ecb"></a>[module crypto-js.mode_ecb](#apidoc.module.crypto-js.mode_ecb)

#### <a name="apidoc.element.crypto-js.mode_ecb.init"></a>[function <span class="apidocSignatureSpan">crypto-js.mode_ecb.</span>init ()](#apidoc.element.crypto-js.mode_ecb.init)
- description and source-code
```javascript
init = function () {
	                        subtype.$super.init.apply(this, arguments);
	                    }
```
- example usage
```shell
...
	            for (var i = 0, rcache; i < nBytes; i += 4) {
	                var _r = r((rcache || Math.random()) * 0x100000000);

	                rcache = _r() * 0x3ade67b7;
	                words.push((_r() * 0x100000000) | 0);
	            }

	            return new WordArray.init(words, nBytes);
	        }
	    });

	    /**
	     * Encoder namespace.
	     */
	    var C_enc = C.enc = {};
...
```



# <a name="apidoc.module.crypto-js.mode_ofb"></a>[module crypto-js.mode_ofb](#apidoc.module.crypto-js.mode_ofb)

#### <a name="apidoc.element.crypto-js.mode_ofb.init"></a>[function <span class="apidocSignatureSpan">crypto-js.mode_ofb.</span>init ()](#apidoc.element.crypto-js.mode_ofb.init)
- description and source-code
```javascript
init = function () {
	                        subtype.$super.init.apply(this, arguments);
	                    }
```
- example usage
```shell
...
	            for (var i = 0, rcache; i < nBytes; i += 4) {
	                var _r = r((rcache || Math.random()) * 0x100000000);

	                rcache = _r() * 0x3ade67b7;
	                words.push((_r() * 0x100000000) | 0);
	            }

	            return new WordArray.init(words, nBytes);
	        }
	    });

	    /**
	     * Encoder namespace.
	     */
	    var C_enc = C.enc = {};
...
```



# <a name="apidoc.module.crypto-js.pad_iso10126"></a>[module crypto-js.pad_iso10126](#apidoc.module.crypto-js.pad_iso10126)

#### <a name="apidoc.element.crypto-js.pad_iso10126.pad"></a>[function <span class="apidocSignatureSpan">crypto-js.pad_iso10126.</span>pad (data, blockSize)](#apidoc.element.crypto-js.pad_iso10126.pad)
- description and source-code
```javascript
pad = function (data, blockSize) {
	        // Shortcut
	        var blockSizeBytes = blockSize * 4;

	        // Count padding bytes
	        var nPaddingBytes = blockSizeBytes - data.sigBytes % blockSizeBytes;

	        // Pad
	        data.concat(CryptoJS.lib.WordArray.random(nPaddingBytes - 1)).
	             concat(CryptoJS.lib.WordArray.create([nPaddingBytes << 24], 1));
	    }
```
- example usage
```shell
...
	         * @param {WordArray} data The data to pad.
	         * @param {number} blockSize The multiple that the data should be padded to.
	         *
	         * @static
	         *
	         * @example
	         *
	         *     CryptoJS.pad.Pkcs7.pad(wordArray, 4);
	         */
	        pad: function (data, blockSize) {
	            // Shortcut
	            var blockSizeBytes = blockSize * 4;

	            // Count padding bytes
	            var nPaddingBytes = blockSizeBytes - data.sigBytes % blockSizeBytes;
...
```

#### <a name="apidoc.element.crypto-js.pad_iso10126.unpad"></a>[function <span class="apidocSignatureSpan">crypto-js.pad_iso10126.</span>unpad (data)](#apidoc.element.crypto-js.pad_iso10126.unpad)
- description and source-code
```javascript
unpad = function (data) {
	        // Get number of padding bytes from last byte
	        var nPaddingBytes = data.words[(data.sigBytes - 1) >>> 2] & 0xff;

	        // Remove padding
	        data.sigBytes -= nPaddingBytes;
	    }
```
- example usage
```shell
...
	         *
	         * @param {WordArray} data The data to unpad.
	         *
	         * @static
	         *
	         * @example
	         *
	         *     CryptoJS.pad.Pkcs7.unpad(wordArray);
	         */
	        unpad: function (data) {
	            // Get number of padding bytes from last byte
	            var nPaddingBytes = data.words[(data.sigBytes - 1) >>> 2] & 0xff;

	            // Remove padding
	            data.sigBytes -= nPaddingBytes;
...
```



# <a name="apidoc.module.crypto-js.pad_iso97971"></a>[module crypto-js.pad_iso97971](#apidoc.module.crypto-js.pad_iso97971)

#### <a name="apidoc.element.crypto-js.pad_iso97971.pad"></a>[function <span class="apidocSignatureSpan">crypto-js.pad_iso97971.</span>pad (data, blockSize)](#apidoc.element.crypto-js.pad_iso97971.pad)
- description and source-code
```javascript
pad = function (data, blockSize) {
	        // Add 0x80 byte
	        data.concat(CryptoJS.lib.WordArray.create([0x80000000], 1));

	        // Zero pad the rest
	        CryptoJS.pad.ZeroPadding.pad(data, blockSize);
	    }
```
- example usage
```shell
...
	         * @param {WordArray} data The data to pad.
	         * @param {number} blockSize The multiple that the data should be padded to.
	         *
	         * @static
	         *
	         * @example
	         *
	         *     CryptoJS.pad.Pkcs7.pad(wordArray, 4);
	         */
	        pad: function (data, blockSize) {
	            // Shortcut
	            var blockSizeBytes = blockSize * 4;

	            // Count padding bytes
	            var nPaddingBytes = blockSizeBytes - data.sigBytes % blockSizeBytes;
...
```

#### <a name="apidoc.element.crypto-js.pad_iso97971.unpad"></a>[function <span class="apidocSignatureSpan">crypto-js.pad_iso97971.</span>unpad (data)](#apidoc.element.crypto-js.pad_iso97971.unpad)
- description and source-code
```javascript
unpad = function (data) {
	        // Remove zero padding
	        CryptoJS.pad.ZeroPadding.unpad(data);

	        // Remove one more byte -- the 0x80 byte
	        data.sigBytes--;
	    }
```
- example usage
```shell
...
	         *
	         * @param {WordArray} data The data to unpad.
	         *
	         * @static
	         *
	         * @example
	         *
	         *     CryptoJS.pad.Pkcs7.unpad(wordArray);
	         */
	        unpad: function (data) {
	            // Get number of padding bytes from last byte
	            var nPaddingBytes = data.words[(data.sigBytes - 1) >>> 2] & 0xff;

	            // Remove padding
	            data.sigBytes -= nPaddingBytes;
...
```



# <a name="apidoc.module.crypto-js.pad_nopadding"></a>[module crypto-js.pad_nopadding](#apidoc.module.crypto-js.pad_nopadding)

#### <a name="apidoc.element.crypto-js.pad_nopadding.pad"></a>[function <span class="apidocSignatureSpan">crypto-js.pad_nopadding.</span>pad ()](#apidoc.element.crypto-js.pad_nopadding.pad)
- description and source-code
```javascript
pad = function () {
	    }
```
- example usage
```shell
...
	         * @param {WordArray} data The data to pad.
	         * @param {number} blockSize The multiple that the data should be padded to.
	         *
	         * @static
	         *
	         * @example
	         *
	         *     CryptoJS.pad.Pkcs7.pad(wordArray, 4);
	         */
	        pad: function (data, blockSize) {
	            // Shortcut
	            var blockSizeBytes = blockSize * 4;

	            // Count padding bytes
	            var nPaddingBytes = blockSizeBytes - data.sigBytes % blockSizeBytes;
...
```

#### <a name="apidoc.element.crypto-js.pad_nopadding.unpad"></a>[function <span class="apidocSignatureSpan">crypto-js.pad_nopadding.</span>unpad ()](#apidoc.element.crypto-js.pad_nopadding.unpad)
- description and source-code
```javascript
unpad = function () {
	    }
```
- example usage
```shell
...
	         *
	         * @param {WordArray} data The data to unpad.
	         *
	         * @static
	         *
	         * @example
	         *
	         *     CryptoJS.pad.Pkcs7.unpad(wordArray);
	         */
	        unpad: function (data) {
	            // Get number of padding bytes from last byte
	            var nPaddingBytes = data.words[(data.sigBytes - 1) >>> 2] & 0xff;

	            // Remove padding
	            data.sigBytes -= nPaddingBytes;
...
```



# <a name="apidoc.module.crypto-js.pad_pkcs7"></a>[module crypto-js.pad_pkcs7](#apidoc.module.crypto-js.pad_pkcs7)

#### <a name="apidoc.element.crypto-js.pad_pkcs7.pad"></a>[function <span class="apidocSignatureSpan">crypto-js.pad_pkcs7.</span>pad (data, blockSize)](#apidoc.element.crypto-js.pad_pkcs7.pad)
- description and source-code
```javascript
pad = function (data, blockSize) {
	            // Shortcut
	            var blockSizeBytes = blockSize * 4;

	            // Count padding bytes
	            var nPaddingBytes = blockSizeBytes - data.sigBytes % blockSizeBytes;

	            // Create padding word
	            var paddingWord = (nPaddingBytes << 24) | (nPaddingBytes << 16) | (nPaddingBytes << 8) | nPaddingBytes;

	            // Create padding
	            var paddingWords = [];
	            for (var i = 0; i < nPaddingBytes; i += 4) {
	                paddingWords.push(paddingWord);
	            }
	            var padding = WordArray.create(paddingWords, nPaddingBytes);

	            // Add padding
	            data.concat(padding);
	        }
```
- example usage
```shell
...
	         * @param {WordArray} data The data to pad.
	         * @param {number} blockSize The multiple that the data should be padded to.
	         *
	         * @static
	         *
	         * @example
	         *
	         *     CryptoJS.pad.Pkcs7.pad(wordArray, 4);
	         */
	        pad: function (data, blockSize) {
	            // Shortcut
	            var blockSizeBytes = blockSize * 4;

	            // Count padding bytes
	            var nPaddingBytes = blockSizeBytes - data.sigBytes % blockSizeBytes;
...
```

#### <a name="apidoc.element.crypto-js.pad_pkcs7.unpad"></a>[function <span class="apidocSignatureSpan">crypto-js.pad_pkcs7.</span>unpad (data)](#apidoc.element.crypto-js.pad_pkcs7.unpad)
- description and source-code
```javascript
unpad = function (data) {
	            // Get number of padding bytes from last byte
	            var nPaddingBytes = data.words[(data.sigBytes - 1) >>> 2] & 0xff;

	            // Remove padding
	            data.sigBytes -= nPaddingBytes;
	        }
```
- example usage
```shell
...
	         *
	         * @param {WordArray} data The data to unpad.
	         *
	         * @static
	         *
	         * @example
	         *
	         *     CryptoJS.pad.Pkcs7.unpad(wordArray);
	         */
	        unpad: function (data) {
	            // Get number of padding bytes from last byte
	            var nPaddingBytes = data.words[(data.sigBytes - 1) >>> 2] & 0xff;

	            // Remove padding
	            data.sigBytes -= nPaddingBytes;
...
```



# <a name="apidoc.module.crypto-js.pad_zeropadding"></a>[module crypto-js.pad_zeropadding](#apidoc.module.crypto-js.pad_zeropadding)

#### <a name="apidoc.element.crypto-js.pad_zeropadding.pad"></a>[function <span class="apidocSignatureSpan">crypto-js.pad_zeropadding.</span>pad (data, blockSize)](#apidoc.element.crypto-js.pad_zeropadding.pad)
- description and source-code
```javascript
pad = function (data, blockSize) {
	        // Shortcut
	        var blockSizeBytes = blockSize * 4;

	        // Pad
	        data.clamp();
	        data.sigBytes += blockSizeBytes - ((data.sigBytes % blockSizeBytes) || blockSizeBytes);
	    }
```
- example usage
```shell
...
	         * @param {WordArray} data The data to pad.
	         * @param {number} blockSize The multiple that the data should be padded to.
	         *
	         * @static
	         *
	         * @example
	         *
	         *     CryptoJS.pad.Pkcs7.pad(wordArray, 4);
	         */
	        pad: function (data, blockSize) {
	            // Shortcut
	            var blockSizeBytes = blockSize * 4;

	            // Count padding bytes
	            var nPaddingBytes = blockSizeBytes - data.sigBytes % blockSizeBytes;
...
```

#### <a name="apidoc.element.crypto-js.pad_zeropadding.unpad"></a>[function <span class="apidocSignatureSpan">crypto-js.pad_zeropadding.</span>unpad (data)](#apidoc.element.crypto-js.pad_zeropadding.unpad)
- description and source-code
```javascript
unpad = function (data) {
	        // Shortcut
	        var dataWords = data.words;

	        // Unpad
	        var i = data.sigBytes - 1;
	        while (!((dataWords[i >>> 2] >>> (24 - (i % 4) * 8)) & 0xff)) {
	            i--;
	        }
	        data.sigBytes = i + 1;
	    }
```
- example usage
```shell
...
	         *
	         * @param {WordArray} data The data to unpad.
	         *
	         * @static
	         *
	         * @example
	         *
	         *     CryptoJS.pad.Pkcs7.unpad(wordArray);
	         */
	        unpad: function (data) {
	            // Get number of padding bytes from last byte
	            var nPaddingBytes = data.words[(data.sigBytes - 1) >>> 2] & 0xff;

	            // Remove padding
	            data.sigBytes -= nPaddingBytes;
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
