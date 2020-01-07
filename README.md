# CyberSecurity
Secure File Storage in Cloud Computing using Hybrid Cryptography Algorithm


In Cloud Computing, we share data among many clients, servers and people. So the
security of information present in cloud is not guaranteed. Thus it is simple for an
intruder to access and demolish the first type of information.
Symmetric Key Cryptography is quick and productive. Anyway, key trade keeps on being
prevention towards its ideal use. The individual who scrambles the message and the
individual, who unscrambles the message in Symmetric Key Cryptography utilize a
similar key and consequently keeping up the security of the regular key, without it
coming into the learning of others, is an extreme inquire. Uneven Key Cryptography is
gainful in annihilating this issue. Here each imparting gathering utilizes two keys to
shape a key pair - one key is made open (and henceforth called open key) that is utilized
to scramble the message.
So, there is a requirement of some plainly key which help us to do cross breed
encryption and protect the data. In the proposed project, half breed encryption is utilized
where records are scrambled by blowfish combined with document part and SRNN
(modified RSA) is utilized for the secured correspondence amongst clients and servers.

Blowfish Algorithm
BlowFish is a symmetric block cipher which uses a Fiestal network, 16 rounds of
iterative encryption and decryption functional design. The block size used is of 64- bits
and key size can vary from any length to 448. Blowfish cipher uses 18 sub arrays each
of 32-bit commonly known as P-boxes and four Substitution boxes each of 32-bit, each
having 256 entries .The algorithm design is shown in figure. It consists of two phases:
one is Key Expansion phase another is Data Encryption phase. In Key expansion
phase, key is converted into several sub-keys and in Data Encryption phase, encryption
occurs via 16-round networks. Each round consists of a key dependent permutation and
a key and data-dependent substitution.

EncryptionEncryption with Blowfish has two primary stages: sixteen cycles of the round function
and yield operation accepting that the given round keys and the estimation of the S-boxes. Subtleties of
how the round keys are produced and S-encloses instated is secured the key timetable
segment.

SRNN Algorithm
SRNN algorithm is similar with RSA with some modification. SRNN algorithm is also a
Public key cryptography algorithm. In this algorithm we have extremely large number
that has two prime factors. In addition to this, we have used two short range natural
numbers in pair of keys. One key (public key) for encryption and other corresponding
key (private key) for decryption. This modification increases the security of the
cryptosystem. So its name is short range natural number public key algorithm.
Key generation Process
● Generate two large random prime p, q.
● Compute n=p*q
● Compute phi=(p-1)*(q-1)
● Choose an integer e, 1 < e < phi, such that gcd(e,phi) = 1 And compute ua
● Find d, such that e*d mod(phi) =1
● Pick short range natural number u randomly such that u < phi-1
● Pick another short range natural number a randomly such that u < a < phi, and
compute ua
● Public key is (n, e, ua
 )
● Private Key is (d, a, u)
p, q, phi should also be kept secret.
Encryption Process
● Obtains the recipient’s public key (n, e, ua
 )
● Represent the plaintext message as positive integer M
● Computes the cipher text C=(m*ua
 )e
 mod n
Send the cipher text C to recipient.
Decryption Process
● Use Recipient private key(d, a , u)
● compute M=(ve*c)d
 mod n where v= uphi-a
 mod n
● Extracts the plaintext from the integer representative M
