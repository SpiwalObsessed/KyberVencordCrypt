# PF2/PV2 / Payload Format V2

In the next update, KVC will used PF2 as the default for sending messages and decoding them. PF1/PV1 messages are still readable, you just won't be able to send them from your PF2/PV2 client.
This encourages updating to the latest userscript version and it benefits everybody. It fixes bugs and increases performance twofold!

## Why am I doing this?
In KVC-PF1, you can tell just by looking at a message, if it's the same message or not. While not very big of a deal or concern, it unfortunately allows 3rd parties to gather messages of the same content together with extremely low effort. This issue isn't taken lightly. As a result, I have created PF2/PV2 which will be released very soon. An update beforehand will be pushed to make the PV1 clients capable of detecting PV2 messages and displaying the boilerplate reason the message can't yet be read.

tl;dr PF2/PV2 stops outsiders gathering messages identical to any outsiders which over time could be used to guess what was said. Not for AES as 1 character changes the whole messages, but character for character identical messages.
