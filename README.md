# Pre-defined DHE groups
This repository contains .pem files for pre-defined DHE groups as recommended by [IETF RFC 7919](https://tools.ietf.org/html/rfc7919) for: 
* `ffdhe4096`
* `ffdhe3072`
* `ffdhe2048`

With the [Internet.nl](https://internet.nl) test tool you can test if your web or mail server uses these parameters for Diffie-Hellman key exchange. 

NCSC-NL considers `ffdhe4096` and `ffdhe3072` to be 'sufficient' and `ffdhe2048` to be 'phase out'. For more information see guideline B6-1 and table 10 for DHE (in English) of the ['IT Security Guidelines for Transport Layer Security (TLS)'](https://english.ncsc.nl/publications/publications/2019/juni/01/it-security-guidelines-for-transport-layer-security-tls) from NCSC-NL.
