
# JWT (Json Web Token) and OAuth2 :


## What is Encryption and Decryption ? 

- Encryption is like locking your message in a box with a secret key, so that nobody else can read it while it’s being sent.

- Decryption is like unlocking that box with the same (or matching) secret key so the person receiving it can read the original message.


## What is Digital Signature ?
- Digital Signature is a type of electronic signature that uses encryption and decryption to verify the authenticity (who sent it) and integrity (not altered) of digital data or messages.

- It proves the sender’s identity and ensures the message hasn’t been changed.


## What is JWT ?
- JWT (JSON Web Token) is a small, secure token used to share information (like user identity) between two parties.

- Structure of JWT:

    - Header → type & algorithm info

    - Payload → the actual data (like user ID, role)

    - Signature → ensures it’s not tampered with
