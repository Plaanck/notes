
## Symmetric Encryption

- A single key is used to both decrypt and encrypt a message.
- The same key can be used many times, or you can generate a new key each time to increase security.
- Overall, this is a pretty unsafe option, as when sending the message to someone else, you need to send the key to them as well, so if someone intercepts that message, they have full access to it.

## Asymmetric Encryption

- Asymmetric Encryption uses two keys, every person has a public key, which anyone has access to, and a private key.
- When you encrypt a message and send it to someone, you use your private key, as well as the recipient's public key.
	- This is referred to as a combined encryption key

- For the recipient to decrypt the message, they would need to use their private key, as well as our public key.
- This is much more secure, as you can be 100% sure that the message is coming from the person who you expect it to come from, due to the "signiture" that this method creates