# nodejs-session-login

To use session in express, it has to use [express-session](https://github.com/expressjs/session). <br/>

From the official documents:
1. Session data is not saved in the cookie itself, just the session ID. Session data is stored server-side. 

2. Since version 1.5.0, the cookie-parser middleware no longer needs to be used for this module to work. This module now directly reads and writes cookies on req/res. Using cookie-parser may result in issues if the secret is not the same between this module and cookie-parser. 

Session store:

In general, session can be saved in :
1. memory storage
2. cookie
3. memory caching, redis or memcached etc
4. database, e.g. mongoDB
