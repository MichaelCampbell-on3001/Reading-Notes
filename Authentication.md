# Authentication

## [Securing Passwords](https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html)

**"BCrypt, IT's SLOW AND STRONG AS H-E-double hockey sticks."**

Bcrypt is a [hash function](https://en.wikipedia.org/wiki/Hash_function) based on a block cipher and introduces a work factor or "security factor".  
Algorithms such as PBKDF2 and BCrypt, [key stretching](https://en.wikipedia.org/wiki/Key_stretching).  


## [Basic Auth](https://en.wikipedia.org/wiki/Basic_access_authentication)

- In Simple terms basic auth is a method for an HTTP user agent to provide a user name and password when making a request.

- It is the simplest technique for enforcing access controls

- The web browser needs to cache credentials for a reasonable period of time to avoid constantly prompting the user.

**Protocol**

**Server Side**
The server needs authentication and requests it by constucting the authenticate header. Below is the anatomy of the **server side authentication process**:
- The WWW-Authenticate header field for basic authentication is constructed as following:

- WWW-Authenticate: Basic realm="User Visible Realm"

- WWW-Authenticate: Basic realm="User Visible Realm", charset="UTF-8"

**Client Side**

WHen the user sends authentication to the server it is constucted in the header filed. Here are those steps.
1. The username and password are combined with a single colon (:). 
2. The resulting string is encoded into an octet sequence. 
3. The resulting string is encoded.
4. Authorization method and a space is then added to the begining of the encoded string.


## [OWASP auth cheatsheet](https://www.owasp.org/index.php/Authentication_Cheat_Sheet)

The above think did not work for me. However, I did find this [resource](https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html).

At the resouce I linked above I found good info on authentication general guide lines, how to implement porper password strength controls and CAPTCHA.




## [bcrypt docs](https://www.npmjs.com/package/bcrypt)

**node.brypt.js** is a library to hash passwords.

You can find a full list of dependencies you will need to use this tool [here](https://github.com/nodejs/node-gyp).

Before running `npm install bcrypt` please make sure you have ALL the needed dependencies.

How to use bcrypt:

It is recommended to use it as follows:

      `const bcrypt = require('bcrypt');
        const saltRounds = 10;
        const myPlaintextPassword = 's0/\/\P4$$w0rD';
      const someOtherPlaintextPassword = 'not_bacon';`

**To hash the password:**

        `bcrypt.genSalt(saltRounds, function(err, salt) {
    bcrypt.hash(myPlaintextPassword, salt, function(err, hash) {
        // Store hash in your password DB.
    });
});`

Keep in mind  the **hashing** done by bcrypt is CPU intensive, so the **sync version** will block the event loop and prevent your application from servicing any other inbound requests or events. The async version uses a **thread pool** which does not block the main event loop.

One of the biggest benefits is the bcrypt comparison function is **not** susceptible to timing attacks.



