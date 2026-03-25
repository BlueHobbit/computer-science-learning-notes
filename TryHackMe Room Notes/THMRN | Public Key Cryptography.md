# Notes
A quick scan through the room makes me think I would be better off looking elsewhere for a thorough explanation of the cryptosystems and the maths behind them but this should serve as a good broad introduction.

The mathematical proof for how the RSA encryption works is informative but doesn't really explain. Okay it requires understanding modular maths which is why.
  - The proof doesn't really explain how the private key is worked out or communicated for the encryption.

A link to modular arithmetic explaation in ENC:BRIT --> https://www.britannica.com/science/modular-arithmetic

A THM challenge where you break poorly set up RSA --> https://tryhackme.com/room/breakrsa

Some tools for cracking rsa encryption (basic):
  - https://github.com/ius/rsatool
  - https://github.com/RsaCtfTool/RsaCtfTool
    - The notes for this tool are fairly intimidating but give the idea that there are multiple attack methods and possibly multiple ways of configuring the RSA algorithm itself.
      - I wonder if my computational algorithms book series have anything about this in them.
     
I think I should do the RSA challenge room once I've gotten over the rest of this room.
As far as I can tell the RSA method essentially creates a mathematical link between the public and private key that is essentially impossible to reverse with sufficiently large numbers involved.
Okay I think I understand it better now because I wasn't considering the origin of the public and private key properly which is through the recipient of the ciphertext. 
In essence, Alice can only send messages for Bob to receive in the example since only Bob has the private key which is used as part of the process for devising the public key pairing that she uses to encrypt. 
  - Assuming far larger primes used for the composite it essentially becomes impossible to reverse the composite by factorising it and thereby prevents another user from working out ϕ(n) which in turn prevents them from working out the private key.
  - The reason I was struggling to understand the security of the algorithm is because for some reason I had assumed the two primes that make the composite would be public for some reason.

Diffie-Hellman seems similar to RSA with the use of modular arithmetic and using the numerous finite possible selections of private keys when arriving at getting your to protect the actual private keys.
- Again there's an emphasis on using even larger numbers than in the example which increases the size of the public keys and creates an even larger number of possible private keys to arrive at the modulus result.
- The actual logic for how Diffie-Hellman works could be more broadly applicable to create a qualitative equivalent to this cryptosystem.

I'm 99% sure I've used ssh-keygen in a different THM room before or a CTF challenge elsewhere though I don't remember the exact context. 
- Tbh this file is mostly highlighting to me how much of an effort it would likely require to get heavily into cryptography and how much my maths skills have gotten a bit rusty since 6th form.

Certificate authorities trusted by Google: https://chromium.googlesource.com/chromium/src/+/main/net/data/ssl/chrome_root_store/root_store.md
Certificate authorities trusted by Firefox: https://wiki.mozilla.org/CA/Included_Certificates

Honorable mention for let's encrypt: https://letsencrypt.org/

Free implementation of the PGP standard with Windows support: https://gnupg.org/

I've heard of John the Ripper but what's gpg2john?#

I feel like steps are missing from the discussion of setting up a new computer with an older GPG signature key.

Getting good at cryptanalysis would probably be a very good way for me to get into CTF competitions.





