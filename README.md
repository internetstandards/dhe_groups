# Pre-defined DHE groups
This repository contains .pem files for the following finite field groups for DHE as standardised by [IETF RFC 7919](https://tools.ietf.org/html/rfc7919): 
* `ffdhe4096`
* `ffdhe3072`

These can be used for configuration of your TLS software. The associated checksums are also published in the test explanation of the 'Key exchange parameters' subtest on Internet.nl. 

The repository does not contain .pem files for `ffdhe2048` as it is 'Insufficient'. Besides, it does not contain .pem files for `ffdhe8192 and `ffdhe61441`, as these are rarely used because of performance loss.

## Testing with Internet.nl
With the [Internet.nl](https://internet.nl) test tool you can test if your web and mail server use these standardised finite field groups for DHE. 

## NCSC-NL TLS Guidelines
Internet.nl uses the ['Transport Layer Security (TLS), Security guidelines version 2025-05'](https://www.ncsc.nl/en/transport-layer-security-tls/security-guidelines-for-transport-layer-security-2025-05) from NCSC-NL as a baseline. NCSC-NL has assigned the following security levels to these groups (paragraph 3.3.3):

### Security level of finite field groups for DHE

* Phase out:

    * `ffdhe8192` (rarely used because of performance loss)
    * `ffdhe6144` (idem)
    * [`ffdhe4096`](https://raw.githubusercontent.com/internetstandards/dhe_groups/master/ffdhe4096.pem) ([RFC 7919](https://www.rfc-editor.org/rfc/rfc7919))  
      sha256 checksum: `64852d6890ff9e62eecd1ee89c72af9af244dfef5b853bcedea3dfd7aade22b3`
    * [`ffdhe3072`](https://raw.githubusercontent.com/internetstandards/dhe_groups/master/ffdhe3072.pem) ([RFC 7919](https://www.rfc-editor.org/rfc/rfc7919))  
      sha256 checksum: `c410cc9c4fd85d2c109f7ebe5930ca5304a52927c0ebcb1a11c5cf6b2386bbab`  
   
* Insufficient:

    * `ffdhe2048`
    * Other groups (i.e. not-standardised, self-generated)
