## 아래 다운받기
 `npm i dotenv http express jsonwebtoken body-parser`
+ dotenv@10.0.0
+ body-parser@1.19.0
+ jsonwebtoken@8.5.1
+ express@4.17.1
+ http@0.0.1-security

## jwt.sign(payload, secretOrPrivateKey, [options, callback])
`payload` could be an object literal, buffer or string representing valid JSON.
`secretOrPrivateKey` is a string, buffer, or object containing either the secret for HMAC algorithms or the PEM encoded private key for RSA and ECDSA. In case of a private key with passphrase an object `{ key, passphrase }` can be used (based on [crypto documentation](https://nodejs.org/api/crypto.html#crypto_sign_sign_private_key_output_format)), in this case be sure you pass the `algorithm` option.
`options` :
 - `expiresIn` : expressed in seconds or a string describing a time span 
                => 기본 단위 ms (ex. 15 -> 15ms)

## 검증사이트
 - [JWT](https://jwt.io/)
 출력된 토큰을 위 사이트에서 넣어보면 HEADER.PAYLOAD.SIGNATURE 형식을 나눠서 보여준다.
