# Bearer Authorization

## [JWTs Explained](https://www.youtube.com/watch?v=926mknSW9Lo)

In basic terms **JWT** allows the user to **securely transmit** information **between parties** as a **JSON object**. It is **digitally signed** along the process which esures it can be **trusted**. 

### The three part structure of JWT
- Header: The **header** typically consists of **two parts**: the type of the **token**, which is JWT, and the **signing algorithm** being used.

-Payload: A **set** of instructions that you want to **include** in the token being generated and/or things your API will need to do.

-Signature: **JWTs** can be **signed** using a **secret** or a **public/private** key pair.

## [Intro to JWT](https://jwt.io/introduction/)

### When should you use JSON Web Tokens?

- Once the user is logged on, they then possess **Authorization** and each request they make will include the JWT. It will alow the user access to the appropriate services and routes. 

- During an **Information exchange** the JWT ensures the data hasn't been tampered with on either end of the transaction. It also allows the senders and receivers to be verified.

WHen you think **tokens** think **credentials**. 

![JWT diagram from the reading](https://cdn2.auth0.com/docs/media/articles/api-auth/client-credentials-grant.png)

## [Are JWTs Secure?](https://stackoverflow.com/questions/27301557/if-you-can-decode-jwt-how-are-they-secure)

So, As far as I understand , the basic concept with JWT is that the three part of the JWT structure are **not** independent. I think the signature is changed when the payload is changed, so if an unauthorized user tries to insert data the new signature would alert the receiver that it may be compromised. How close am I? 