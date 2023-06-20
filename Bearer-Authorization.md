# Bearer Authorization

## [Intro to JWT](https://jwt.io/introduction/)

### What is a JSON Web Token (JWT)?

JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.

### When should we use JSON Web Tokens?

* **Authorization**: This is the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token.

* **Information Exchange:** JSON Web Tokens are a good way of securely transmitting information between parties. Because JWTs can be signed—for example, using public/private key pairs—you can be sure the senders are who they say they are.
### Claims are expected in which structural component of a JWT?

note that claims are: Claims are statements about an entity (typically, the user) and additional data. There are three types of claims: registered, public, and private claims.


Claims are expected to be present in the payload component of a JSON Web Token (JWT). 

## [Are JWTs Secure?](https://stackoverflow.com/questions/27301557/if-you-can-decode-jwt-how-are-they-secure)

### If I get a JWT and I can decode the payload, how can we call that secure?

WTs can be either signed, encrypted or both. If a token is signed, but not encrypted, everyone can read its contents, but when you don't know the private key, you can't change it. Otherwise, the receiver will notice that the signature won't match anymore.

Let's assume Alice wants to send a JWT to Bob. They both know some shared secret. Mallory doesn't know that secret, but wants to interfere and change the JWT. To prevent that, Alice calculates Hash(payload + secret) and appends this as signature.

When receiving the message, Bob can also calculate Hash(payload + secret) to check whether the signature matches. If however, Mallory changes something in the content, she isn't able to calculate the matching signature (which would be Hash(newContent + secret)). She doesn't know the secret and has no way of finding it out. This means if she changes something, the signature won't match anymore, and Bob will simply not accept the JWT anymore

### If sending a JWT, what must sender and receiver both know? Hint, it’s appended in the signature.
they both should know a shared secret between them 
Hash(payload + secret)
when hashing the payload which contains the data you want to send it will concatinated with the secret as a single string then hashed using hashing function the reciever should be abble to recalculate the value of hashing since he knows the secret 

### Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter.

Let's assume Alice wants to send the JWT to Bob, and they have a shared secret of "mySecretKey". The payload is: {"message": "Hello Bob!"}. Alice will calculate the signature as follows:

Concatenate the payload and the shared secret:
Payload: {"message": "Hello Bob!"}
Shared Secret: "mySecretKey"
Concatenated String: '{"message": "Hello Bob!"}mySecretKey'

Apply a hash function (e.g., HMAC-SHA256) to the concatenated string:
Signature: HMAC-SHA256('{"message": "Hello Bob!"}mySecretKey')

The resulting signature will be a unique value derived from the concatenation of the payload and the secret key using the chosen hash function.

Alice now sends the JWT to Bob, containing the payload and the signature.

Upon receiving the JWT, Bob extracts the payload and the received signature. Bob knows the shared secret ("mySecretKey") and can now verify the integrity of the payload by recalculating the signature as follows:

Concatenate the received payload and the shared secret:
Payload: {"message": "Hello Bob!"}
Shared Secret: "mySecretKey"
Concatenated String: '{"message": "Hello Bob!"}mySecretKey'

Apply the same hash function (HMAC-SHA256) to the concatenated string:
Recalculated Signature: HMAC-SHA256('{"message": "Hello Bob!"}mySecretKey')

Bob then compares the recalculated signature with the received signature. If the two signatures match, it means the payload hasn't been tampered with during transit, and Bob can trust the integrity of the message. If the signatures don't match, Bob can conclude that the JWT has been modified, and he should reject it.

The process of calculating and verifying the signature ensures that the JWT remains secure and tamper-proof, providing authentication and data integrity between Alice and Bob.


## [JWTs Explained](youtube.com/watch?v=926mknSW9Lo)

### Why use JWT?

 JWTs provide security through cryptographic signatures, ensuring data integrity and authenticity.

### JWT is Compact and self-contained. Describe how this is useful to a non-technical friend.


Imagine you have a special keychain that can hold all your important information securely. This keychain is compact and easy to carry around. It contains everything you need, like your ID, membership cards, and even some personal notes.

Now, let's say you want to access a service or enter a place that requires identification. Instead of carrying multiple documents or remembering various usernames and passwords, you can simply show your keychain. It contains all the necessary information in one place.

### What are the three components (the structure) of a JWT signature?

the header, payload and signiture