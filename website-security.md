### title: web security: improvements for any website
### speaker: RB Woods
### date: 08102019

##### notes:
- email address/password
- password hashing might not be done right
- target hack: thermostat hack (on same network) => point of sale system
- sql injection: 
  - almost dead
  - prepared statements
- sessions:
  - expire them often
  - renew/refresh with activity
- cookies:
  - encrypt data in it
- passwords:
  - any char should be allowed
  - length is vital and most important
  - encourage 2FA
  - part of company: 2FA hardware tokens (ubikey)
- password storage:
  - store the hash
  - language built in encryption libraries
  - sso (facebook/google) with oauth2: problem if google account gets hacked
  - consider 2/3 step login process
  - dont do sms as it can be attacked; use google authenticator
- https:
  - lets encrypt: free cert
- csrf mitigation:
  - performs unwanted action against a trusted site when authenticated
  - xss is not necessary for csrf
  - csrf mitigation techniques
  - dont do critical transactions via GET
  - <img src> tags
  - any state changing operation requires a secure random csrf token
  - look at owasp first
  - csrf token needs to get pushed at the last min so that dangerous js can read those tokens
  - any xss vulenrabaility can defeat any xss
- xss:
  - access cookies, sessions, impersonation
  - same origin policy
  - embedded 3rd party scripts might have dangerous embedded scripts
  - csp (content security policy): no one seems to be using but inline js is disabled by default
  - csp; whitelisting doesnt work => hard to maintain => causes breakages
  - csp; nonce based used in script-src => only 0.92% are using it
  - csp; research and implement this
  - xframe options
  - X-content type options
  - HSTS

