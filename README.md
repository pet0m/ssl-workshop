# SSL Workshop

In browser SSL workshop.

## Certificate Signing Request (CSR)
For the moment, this is the only implemented feature for the moment.

It is a single purpose no CSR generator, which allows to set certificate's subject Common Name (CN) and allows to set certificate's Subject Alternative Names (SANs) with DNS and IP values.
It is meant for quick and easy CSR generation for people not familiar with OpenSSL tool or any other PKI tools.

Generated private key is an RSA 4096 bit key with SHA256 fingerprint and usage is set for "sign" and "verify".

CSR is generated with keyUsage attribute set to "Digital Signature, Key Encipherment".

It is a completely stand-alone HTML file. It does not load any external Javascript and can be open straight from a file explorer into the web browser. Does not require a web server to be used.

It uses web browser's embedded `crypto` library. 


## TODO:
Self-signed certificate generator with export to PEM file.
