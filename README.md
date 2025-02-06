## OpenSSL on AmpereOne
OpenSSL supports AmpereOne processors.  
To better leverage the new features(SHA3,SHA512) introduced by AmpereOne, OpenSSL version 3.4.0 is recommended.  
[Commit](https://github.com/openssl/openssl/commit/e7f1afe4f7e799394684ce86bd98f2445031eb7f) provides the optimization for AmepreOne by using the loop unrolling and EOR3 instructions.

For other versions, like 3.2.x and 3.3.x, we provided a version with the patch backported. 
- version 3.2.3: [branch openssl-3.2.3](https://github.com/AmpereComputing/openssl/tree/openssl-3.2.3)
- version 3.3.2: [branch openssl-3.3.2](https://github.com/AmpereComputing/openssl/tree/openssl-3.3.2)
