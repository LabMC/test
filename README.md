# test
===Basic Authorization Header===
# FP Checker to prevent this scan if the terms "Login", "Signin", or "Signup appear.
+Issue Detail:
This web application appears configured to use the "Basic" HTTP authentication scheme for authenticating HTTP requests.
Use of the "Basic" authentication scheme involves directly sending user credentials over an HTTP request in plaintext.
Because the "Basic" scheme type requires clients to send credentials over an HTTP request in plaintext, it becomes highly-suggested to avoid its use whenever possible.
Use of the "Basic" HTTP request (if necessary) should only be restricted for when users must directly send credentials to servers (such as "Login" or "Sign-Up" webpages).
Alternatives include: Bearer, Digest.
+Issue Remediation:
Plaintext disclosure in an HTTP request should only be acceptable during "Login" or "Sign-Up" web processes.
Usage of credentials should be avoided whenever possible to avoid potential breach attacks (MITM) from arising.
Rather, best practice suggests recommends involving processes which allow the web server to first perform internal encryption & gain approval with the intended server using this ciphertext.
+Issue Advice:
- Bearer Authentication Scheme: Used for sending credentials over customized token methodology (often via the OAuth 2.0 & OpenID Connect frameworks).
- Digest Authentication Scheme: Used for sending credentials over MD5 encryption values.



+Issue Detail:
This web application appears configured to use the "Password" grant type for authenticating OAuth 2.0 HTTP requests.
Use of the "Password" grant type in an "OAuth 2.0" HTTP authentication scheme involves directly sending user credentials towards an intended authentication server in plaintext.
Because the "Password" grant type requires clients to send credentials over an HTTP request in plaintext, it becomes highly-suggested to switch this code grant out with an encrypted alternative.
Examples include: Authorization, Client Credentials.
+Issue Remediation:
Plaintext disclosure in an HTTP request should only be acceptable during "Login" or "Sign-Up" web processes.
Usage of credentials should be avoided whenever possible to avoid potential breach attacks (MITM) from arising.
Rather, best practice suggests recommends involving processes which allow the web server to first perform internal encryption & gain approval with the intended server using this ciphertext.
+Issue Advice:
- Authorization Code Grant: Used for External S2S & Internal S2S.
- Client Credentials Code Grant: Used for Internal S2S.
- Device Code Grant: –Used for Browserless S2S (IOT devices).


