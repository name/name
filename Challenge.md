## The Challenge Process

To verify that who you're talking to is actually me, feel free to challenge my identity at any time. The simplest way to do this is by sending me an identity challenge, which is a message containing random secrets of your choosing that you'll encrypt using my [PGP Public Key](README.md#PGP). You can see an unencrypted example of such a challenge below:

---

<details>
  <summary><strong>Example Challenge</strong></summary>

<pre>
I want to verify that you're actually Charlie Maddex. Therefore, I've encrypted this message using your public key.

I've chosen a random secret that only you'll be able to reveal by decrypting this message with your access card's private key.

The random secret is simply three randomly generated UUIDs, which I've saved locally so I can verify them later:
<strong>87a19c41-f7bb-47f9-9aaf-5884e5f35bed</strong>
<strong>efa7dbbb-ea86-42d8-ac65-58a5990d4cfc</strong>
<strong>ca027737-41e7-4922-b1f5-27c73774560c</strong>

Because anyone impersonating you can simply send this message to you and then pass your response to them along to me, please make sure you only respond to this challenge from the following username/platform:
<strong>Telegram: @username</strong>

The current epoch time is <strong>1595792255</strong>. I understand that you won't reply to this message if there's too much time between the time this message was encrypted and the time you receive it.

I also understand that if there's malware on my computer at the time of me encrypting this message, it's possible a bad actor may already have the plaintext version of this message.
</pre>
</details>

---

## Sending a Challenge

If you're ready to challenge my identity, please follow the steps outlined below.

### Step 1. Preparing the Challenge

<sub></sub>

---

<details>
<summary><strong>Copy and Update the Challenge Template</strong></summary>

Copy the challenge template below to a notepad or text editor. The data that needs to be updated is in <strong>bold</strong> and is surrounded by asterisks. If you're not sure if you're doing it right, you can always compare your challenge to the "Example Challenge" above.
 
<pre>
I want to verify that you're actually Charlie Maddex. Therefore, I've encrypted this message using your public key.

I've chosen a random secret that only you'll be able to reveal by decrypting this message with your access card's private key.

The random secret is simply three randomly generated UUIDs, which I've saved locally so I can verify them later:
<strong>*insert <a href="https://onlinerandomtools.com/generate-random-uuid?count=3">3 Random UUIDs</a> here*</strong> // BE SURE TO SAVE THESE LOCALLY SO YOU CAN VERIFY THEM LATER!

Because anyone impersonating you can simply send this message to you and then pass your response to them along to me, please make sure you only respond to this challenge from the following username/platform:
<strong>*insert your username and platform here*</strong> // If the platform uses a discriminator (user#1234), be sure to include it!

The current epoch time is <strong>*insert <a href="https://www.epochconverter.com/">current epoch time</a>*</strong>. I understand that you won't reply to this message if there's too much time between the time this message was encrypted and the time you receive it.

I also understand that if there's malware on my computer at the time of me encrypting this message, it's possible a bad actor may already have the plaintext version of this message.
</pre>

</details>

---

<details>
<summary>Why do I need to specify secret data and save it locally?</summary>
<br>

Once you encrypt the secret data, it can only be decrypted by my private key. This means that somebody who is pretending to be me won't be able to tell you what the secrets are. I've chosen to use 3 UUIDs because they're simple and because there are a possible 2<sup>122</sup> UUIDs.

The reason you'd save them locally is so you can verify that the secrets I've decrypted are actually the ones you sent to me (thus, verifying my identity).

You can generate [3 Random UUIDs](https://onlinerandomtools.com/generate-random-uuid?count=3). Alternatively, you can use [random.org](https://random.org) for UUID generation, or you can provide any other sufficiently random piece of text.

</details>

---

<details>
<summary>Why do I need to specify my username and platform?</summary>
<br>

If you send a challenge to somebody who is pretending to be me, there would be nothing stopping them from taking your challenge and sending it to me. If that happened, I'd respond to them with the secrets, and they could respond to you with them. To avoid this, I'll only provide the decrypted secrets to the username on the platform provided here.

If this is a platform that uses a username discriminator (e.g. Test#1234), be sure to include your discriminator. If the platform uses a discriminator and you do not provide one, I will not provide you with the decrypted secrets.

</details>

---

<details>
<summary>Why do I need to provide the current epoch timestamp?</summary>
<br>

To ensure that messages aren't [replayed](https://en.wikipedia.org/wiki/Replay_attack), or that an impersonator doesn't make excuses as to why they cannot decrypt the message for a certain period of time:

 - I won't provide decrypted secrets for any message that isn't carrying a timestamp.
 - I may not respond if too much time has passed between the timestamp and the time I receive the message. (We're talking about several hours, not seconds or minutes)

</details>

---

### Step 2. Encrypt the Message

Now that you've updated all of the challenge data, you can encrypt it. Simply choose which option below best describes you:

---

<details><summary>I already know how to use PGP, just give me your public key.</summary>
<br>

Jeez, okay. You can find my public key [here](README.md#PGP). Just be sure to save your encrypted message as `challenge.txt` and send it to me on the respective platform. Alternatively, you can send me a link to a [Gist](https://gist.github.com/new) or [Hastebin](https://hastebin.com/).

</details>

---


<details><summary>I have no idea how to use PGP, help me!</summary>
<br>

You can [quickly encrypt your message](https://pgp.help/#/permalink?pgp=-----BEGIN%20PGP%20PUBLIC%20KEY%20BLOCK-----%0D%0AVersion:%20OpenPGP.js%20v1.5.7%0D%0AComment:%20https:~2F~2Fpgp.help%0D%0A%0D%0AxsBNBF8d3i4BCAC4CKhQn1kIy1aQ8rRXQlA9ybVrhV6UWNu%2BOOre6V7uhf%2B1%0Ae7dHqFFBcwOzZ6ART1dxaEPPbVT2743yIif2El2iXoTrHd95BcNZ2BBfGwB9%0AK7v9TXg9qmj5Q~2FUW3xQ7bOeJ14aAdJnMh1EKoPqLTcUX0rLuWAce~2FCp~2F2jRm%0A48z5%2BssGgpUqiYFbQNG5Tj8RjPhHZVfyHIL8rr39BZ%2Bf3p4wsLg7Td%2BQQTQr%0AaLZj7Qwz3kFd~2FwcIIGW8Jj6IEdb%2ByYoG~2FP%2BbG%2BhyqB30daSOI95tvWIHbp5L%0AOp53RDJZJv0kWlu69nZQBeSPX4nH0GPrMdsR1uc8eAGmObdxOInrC54PABEB%0AAAHNH0NoYXJsaWUgTWFkZGV4IDxldGhAcmlzZXVwLm5ldD7CwHUEEAEIACkF%0AAl8d3i4GCwkIBwMCCRCtp7aHRKqA2wQVCAIKAxYCAQIZAQIbAwIeAQAAXlcH%0A~2FiRSOKdAnAh0MhA9JzQaqmHpP8QrU9uMENMuZ89UGbxb9kvtzx~2FVBD%2BpyBgi%0AooaZxgTv4erWKxWB65kUqV0LJgaCVBag1bOgmigB0w2ZTqhLTT~2F2ZoeBXbYN%0AooEcY9skT7adzxEGas3meVVju2zMTjwB7f%2BQ6QtnsveaPf~2FMiU8LsjmslbMP%0AExkz5p0Yk5cMRN9Z6ZTaFhPSr0tDWnCwBxbah1hbURdw6vS%2B%2Bc8n3e~2F~2FGNhy%0AjtYxv2A1l%2B8YDzBBC3WP21dGuLtgH~2FneULzvU7fezLwY0Oa8WHA8FFHSwEL7%0ATtbCRY3kqotaB8y009ltMz7bAMKk0gf8KYtwTP38fiHOwE0EXx3eLgEIAKHi%0ALUwY88ZhJmxmJDns~2FS1IS~2FpyuFUS2TNl38QT2bmGKPzEk73Uq4PfYZgg50OH%0ApB7wi2X0G59kUNoYoWCk63UvTfJ9F6ZOpAyA~2FNbGT3jn5RMVHlmANAVSUVPm%0AQyLs4~2F1EVb~2F7uzdzJrWyNAW0e6bN2R~2FFilkwhDYZeivthNgLN9N8eo%2B9XQds%0Ado8DBbTKyv1SuGZ0IkmE3PSOcm6ZZSjQYACynoD92qGyxMJ3aZS%2B9Drb75XS%0Aoa4yMSFbob9GM6fBCs26WkmK7n6XpgJpUE1QDGQObsWywrVbCdYU5~2FRvYsX1%0AxtMgNYKUoLYickfzaUoAUh8O3CjCugRgW2sulfUAEQEAAcLAXwQYAQgAEwUC%0AXx3eLwkQrae2h0SqgNsCGwwAAGmrCACWlm5Lg0RHevs4mdcmI3aF%2BxP6HKSG%0ANdnkDPFrJ~2F8Gb4S6oBQr6bxw7Od8P6ly9H7ntfRPxtTV6ZjAHMkr95F8HR0V%0ADDCyOwMjbqtZXnB5xGbekhwFEGW%2B8x3QsyaduMQdHKwTMIiZ1CD2AZ9n42~2F3%0AlNqldCsOmtsnGfIV63oGoAazB3oDDx%2BO8b~2F7BRSqLnEH9dzklrODhGVuGK1L%0AKUaz4rOq59XcMltmW4D6Gzt1vWU4uPBpHbQgmXRUc4VIGNY8voxun~2Fusgm37%0AYWisloMoBlfvRiVXM7bokSXQjIlT3tErpLlzAd4vToHP01Bc7rRx4D8Aj1Ns%0AtKrJuVEqgliU%0D%0A%3DYx4I%0D%0A-----END%20PGP%20PUBLIC%20KEY%20BLOCK-----%0D%0A%0D%0A) using pgp.help (this link is set to encrypt data using my public key.)

**Please don't use this link for anything other than challenges.** If you are sending data that contains PII or other sensitive information, please properly configure PGP locally. **Before entering any text on pgp.help,** please verify that the source code contains the following header, which at the time of writing appears on line 12 and will ensure that your data is not transmitted over the internet:

```
<meta http-equiv="Content-Security-Policy" content="default-src 'none'; script-src 'self'; style-src 'self'; font-src 'self'; img-src 'self';">
```

Once you've verified this, simply copy the data from your notepad or text editor to the "**Message**" section. In the result section, you'll see something like this (but much larger):

```
-----BEGIN PGP MESSAGE-----
Version: OpenPGP.js v1.5.7
Comment: https://pgp.help

wcFMAywoH9voh9j9ARAAjKmuv64sF/uFyPmxgmEkR2Jaul/++22zJsyLxgOt
YsIJMaWwzAkHMasvfTQ0RwW1L3y+5DDhGVKOm9tWTUXqOBtyWcwa+9wGZCF/
y77n+k9/sYVVb
=o3ti
-----END PGP MESSAGE-----
```

Copy the result and save it as `challenge.txt`. Then, send me the challenge.txt file on the respective platform. Alternatively, you can send me a link to a [Gist](https://gist.github.com/new) or [Hastebin](https://hastebin.com/).

</details>

---

## Other Notes

If "I can't respond to the challenge" or for some other reason can't give you your secrets (except as specifically outlined above), you can be sure you're not actually talking to me.

I can promise you that neither the CheatBreaker client nor its source code are for sale. Anybody claiming to sell either of these is either scamming you, violating their non-disclosure agreements, or committing theft of trade secrets. In any case, your best bet is to save your money and not go down that rabbit-hole.

To be clear, it's still possible that an attacker could, in theory, retrieve your secrets without having access to my private key. If you're interested in how that may be, see the _"How!?!"_ section below:

---

<details><summary>How!?!</summary>
<br>

For example, one could attack the UUID generator website I've mentioned. That's possible, but unlikely, and there's not an extremely reliable way to figure out which secrets were actually used in your challenge.

An attacker could go after pgp.help, which would be much more useful than going after the UUID generator website. However, if you check the source code and verify that the Content-Security-Policy is intact, this _should_ stop most attacks. Even so, this attack is easily thwarted by using something such as [Gpg4win](https://www.gpg4win.org/) or another native implementation of PGP.

An attacker could have malware on your device, and would be able to see the data prior to encryption or see the secrets you saved. This is probably the most useful for an attacker, as they'd pick the data up prior to it having been encrypted.

Alternatively, you could have attracted the attention of a nation-state... In which case, what the hell did you do?
</details>

---

<details>
<summary>pgp.help</summary>
<br>

pgp.help is a couple of years old, but it should be fine for a simple challenge use-case such as this.

Please don't use pgp.help for anything other than challenges, though. If you are sending data that contains PII or other sensitive information, please properly configure PGP locally. Before entering any text on pgp.help, please verify that the source code contains the following header, which at the time of writing appears on line 12 and will ensure that your data is not transmitted over the internet:

```
<meta http-equiv="Content-Security-Policy" content="default-src 'none'; script-src 'self'; style-src 'self'; font-src 'self'; img-src 'self';">
```

If you want your challenge to be more secure, then you can encrypt the challenge yourself using [my public key](README.md#PGP).

</details>

---

**In any case, this process is still extremely effective at snuffing out the idiots who are running Minecraft servers and clients pretending to be me.**
