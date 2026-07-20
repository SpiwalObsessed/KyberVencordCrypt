# Missing Decryption Key
If you're here, it's most likely you clicked on the new fancy embed that shows your message is missing a decryption key.

## What's a decryption key?
Good question. However, simple knowledge of cryptography is important when using something like KVC. Keep this in mind. If you do not have this kind of knowledge or find this too confusing, I suggest switching platforms. For example, to Signal.
A decryption key is basically a key which you need to decrypt the encrypted message you're trying to read.

If I _encrypt_ a message, i'm taking its contents and making it look ~99.9% indistinguishable from random white noise / data. Without the correct decryption key, I cannot read the message.
If I encrypt Hello, World! with AES and the hex data for its output is for example 7cae9f1290391ea4bf3b4e50cf5396dd i cannot decrypt the message back to Hello, World! Without prior or newly found knowledge of its decryption key. As decryption with the wrong key even 1 character off will output data which once again just looks like white noise and nothing else.
The idea is encryption provides you the end user with plausable deniability up to a certain degree given your encryption keys are stored in the local device database protected with a secure password. This encrypts your keybag, locking it away from malicious actors. Even yourself if you lose the password to your database, be careful!

## Can I read the message without the decryption key?
Absolutely not. It's impossible to bruteforce an AES-256 key. Because if you try, it would take until the heat death of the universe even with powerful supercomputers.

## I need to read the message. What do I do now?
You can:
* Ask the message author to share the key with you by right clicking the lock icon and clicking share keys.
* Initiate a key exchange and securely ask them to send you the message through direct messages.
* Ask for a screenshot of the message from their client (NOT recommended. This breaks the idea of hiding the messages from Discord and outsiders in the first place.)

## What is Payload Format V2?
You're on the wrong document. see [What is Payload Format V2?](https://github.com/SpiwalObsessed/KyberVencordCrypt/blob/main/PayloadFormatV2.md) for more information.
