# KyberVencordCrypt
KyberVencordCrypt is a fork of SimpleDiscordCrypt Extended!
It fixes the broken plugin altogether, and now uses webpack for a smaller file!
Not only that, but it now uses a PQC Algorithm for key exchange called Kyber-1024.
That might not mean much to anyone but it means your secrets are safe as long as you have a strong database password.

## OTHER UPDATES:
KyberVencordCrypt now uses the recommended amount of Password Iterations recommended by PBKDF2 to hash the password.
Before: 1x sha2-512
After: 600k sha2-512
While this isn't PBKDF2, it's much, much more secure than before!

## NOTICE:
KyberVencordCrypt ONLY runs on Vencord Web as of now. Sorry!

## INSTALLATION
To install, please install Tampermonkey from https://www.tampermonkey.net/ and then click [here](https://github.com/SpiwalObsessed/KyberVencordCrypt/raw/refs/heads/main/KyberVencordCrypt.user.js) to install the userscript!

## WARNING
If you do not encrypt your database with a password, KyberVencordCrypt is basically useless, as physical access to any devices would compromise messages.
Key rotations happen every 24 hours just like before. This does not effect the ability to read older messages!
