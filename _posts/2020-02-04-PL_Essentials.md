# Essentials

## Authentication

- Cookies can be manipulated to change values, which can lead to vulnerabilities
- Cookies sometimes have values that are encoded
- DB lookups can be abused if misconfigured to allow, variants of a registered username to allow access to a different users (admin -> aDmin)
  - Comparison is not case sensitive 
  - Can also be used with spaces (admin -> admin_ )
- Using Burp a misconfigured page can present it's source code in the Response

