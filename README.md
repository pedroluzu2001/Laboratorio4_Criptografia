# Lab 4 - Assyemtric Key

Objective: The key objective of this lab is to provide a practical introduction to public key 
encryption, and with a focus on RSA and Elliptic Curve methods. This includes the creation of 
key pairs and in the signing process.

## A._ RSA Encryption
### A.1 The following defines a public key that is used with PGP email encryption:*


-----BEGIN PGP PUBLIC KEY BLOCK-----
Version: GnuPG v2
```
mQENBFTzi1ABCADIEWchOyqRQmU4AyQAMj2Pn68Sqo9lTPdPcItwo9LbTdv1YCFz
w3qLlp2RORMP+Kpdi92CIhdUYHDmZfHZ3IWTBgo9+y/Np9UJ6tNGocrgsq4xWz15
4vX4jJRddC7QySSh9UxDpRWf9sgqEv1pah136r95ZuyjC1EXnoNxdLJtx8PliCXc
hV/v4+KfOyzYh+HDJ4xP2bt1S07dkasYZ6cA7BHYi9k4xgEwxVvYtNjSPjTsQY5R
cTayXveGafuxmhSauZKiB/2TFErjEt49Y+p07tPTLX7bhMBVbUvojtt/JeUKV6vK
R82dmOd8seUvhwOHYB0JL+3S7PgFFsLo1NV5ABEBAAG0LkJpbGwgQnVjaGFuYW4g
KE5vbmUpIDx3LmJ1Y2hhbmFuQG5hcGllci5hYy51az6JATkEEwECACMFAlTzi1AC
GwMHCwkIBwMCAQYVCAIJCgsEFgIDAQIeAQIXgAAKCRDsAFZRGtdPQi13B/9KHeFb
l1AxqbafFGRDEvx8UfPnEww4FFqWhcr8RLWyE8/COlUpB/5AS2yvojmbNFMGzURb
LGf/u1LVH0a+NHQu57u8Sv+g3bBthEPh4bKaEzBYRS/dYHOx3APFyIayfm78JVRF
zdeTOOf6PaXUTRx7iscCTkN8DUD3lg/465ZX5aH3HWFFX500JSPSt0/udqjoQuAr
WA5JqB//g2GfzZe1UzH5Dz3PBbJky8GiIfLm0OXSEIgAmpvc/9NjzAgjOW56n3Mu
sjVkibc+lljw+rOo97CfJMppmtcOvehvQv+KG0LZnpibiWVmM3vT7E6kRy4gEbDu
enHPDqhsvcqTDqaduQENBFTzi1ABCACzpJgZLK/sge2rMLURUQQ6l02UrS/GilGC
ofq3WPnDt5hEjarwMMwN65Pb0Dj0i7vnorhL+fdb/J8b8QTiyp7i03dZVhDahcQ5
8afvCjQtQstY8+K6kZFzQOBgyOS5rHAKHNSPFq45MlnPo5aaDvP7s9mdMILITvlb
CFhcLoC6Oqy+JoaHupJqHBqGc48/5NU4qbt6fB1AQ/H4M+6og4OozohgkQb80Hox
YbJV4sv4vYMULd+FKOg2RdGeNMM/aWdqYo90qb/W2aHCCyXmhGHEEuok9jbc8cr/
xrWL0gDwlWpad8RfQwyVU/VZ3Eg3OseL4SedEmwOO
cr15XDIs6dpABEBAAGJAR8E
GAECAAkFAlTzi1ACGwwACgkQ7ABWURrXT0KZTgf9FUpkh3wv7aC5M2wwdEjt0rDx
nj9kxH99hhuTX2EHXuNLH+SwLGHBq5O2sq3jfP+owEhs8/Ez0j1/fSKIqAdlz3mB
dbqWPjzPTY/m0It+wv3epOM75uWjD35PF0rKxxZmEf6SrjZD1sk0B9bRy2v9iWN9
9ZkuvcfH4vT++PognQLTUqNx0FGpD1agrG0lXSCtJWQXCXPfWdtbIdThBgzH4flZ
ssAIbCaBlQkzfbPvrMzdTIP+AXg6++K9SnO9N/FRPYzjUSEmpRp+ox31WymvczcU
RmyUquF+/zNnSBVgtY1rzwaYi05XfuxG0WHVHPTtRyJ5pF4HSqiuvk6Z/4z3bw==
=ZrP+
```
-----END PGP PUBLIC KEY BLOCK-----

### Using the following Web page, determine the owner of the key, and the ID on the key:
https://asecuritysite.com/encryption/pgp1

### By searching on-line, can you find the public key of three famous people, and view their key  details, and can you discover some of the details of their keys (eg User ID, key encryption method, key size, etc) 
-----BEGIN PGP PUBLIC KEY BLOCK-----
```

mQENBFxEQeMBCACtgu58j4RuE34OW3Xoy4PIXlLv/8P+FUUFs8Dk4WO5zUJN2NfN
45fIASdKcH8cV2wbCVwjKEP0h4p5IE+lrwQK7bwYx7Qt+qmrm5eLMUM8IvXA18wf
AOPS7XeKTzxa4/jWagJupmmYL+MuV9o5haqYplOYCcVR135KAZfx743YuWcNqvcr
3Em0+gh4F2TXsefjniwuJRGY3Kbb/MAM2zC2f7FfCJVb1C30OLB+KwCddZP/23ll
nOqmzaVF0qQrHQ5EZGK3j3S4fzHNq14TMS3c21YkPOO/DV6BkgIHtG5NIIdVEdQh
wV8clpj0ZP7ShIE8cDhTy8k+xrIByPUVfpMpABEBAAG0J0JpbGwgQnVjaGFuYW4g
PHcuYnVjaGFuYW5AbmFwaWVyLmFjLnVrPokBVAQTAQgAPhYhBK9cqX/wEcCpQ6+5
TFPDJcqRPXoQBQJcREHjAhsDBQkDwmcABQsJCAcCBhUKCQgLAgQWAgMBAh4BAheA
AAoJEFPDJcqRPXoQ2KIH/2sRAsqbrqCMNMRsiBo9XtCFzQ052odbzubIScnwzrDF
Y9z+qPSAwaWGO+1R3LPDH5sMLQ2YOsNqg8VvTJBtOjR9YGNX9/bqqVFRKKSQ0HiD
Sb2M7phBdk4WLkqLZ/AfgHaLKpfNX0bq7WhqZ+Pez0nqjN08JkIog7LhaQZh/Chf
0pl+wHV0rEFuaDQn83yF5DWB1Dt4fbzfVUrEJb92tSrReHALQQA3h5WkTA0qxhDd
9XyEWknDrYCWIWoj0XWjiVUre2fw3SKn8KHvJDeDYVKzYy18oA+da+xgs9b+n+Tq
mMlfslWhw9wRyp0jbVLEs3yxLgE4elbCCmgiTNpnmMW5AQ0EXERB4wEIAKCPJqmM
o8m6Xm163XtAZnx3t02EJSAV6u0yINIC8aEudNWg+/ptKKanUDm38dPnOl1mgOyC
FEu4qFJHbMidkEEac5J0lgvhRK7jv94KF3vxqKr/bYnxltghqCfXesga9jfAHV8J
M6sx4exOoc+/52YskpvDUs/eTPnWoQnbgjP+wsZpNq0owS6yO5urDfD6lvefgK5A
TfB9lQUE0lpb6IMKkcBZZvpZWOchbwPWCB9JZMuirDSyksuTLdqgEsW7MyKBjCae
E/THuTazumad/PyEb0RCbODdMb55L6CD2W2DUquVBLI9FN6KTYWk5L/JzNAIWBV9
TKfevup933j1m+sAEQEAAYkBPAQYAQgAJhYhBK9cqX/wEcCpQ6+5TFPDJcqRPXoQ
BQJcREHjAhsMBQkDwmcAAAoJEFPDJcqRPXoQGRgH/3592g1F4+WRaPbuCgfEMihd
ma5gplU2J7NjNbV9IcY8VZsGw7UAT7FfmTPqlvwFM3w3gQCDXCKGztieUkzMTPqb
LujBR4y55d5xDY6mP40zwRgdRlen2XsgHLPajRQpAhZq8ZvOdGe/ANCyXVdFHbGy
aFAMUfAhxkbITQKXH+EIkCHXDtDUHUxmAQvsZ8Z+Jm+ZwdhWkMsK43tw8UXLIynp
AeOoATdohke3EVK5+0Dc/jezcUWz2IKfw7LB3sQ4c6H8Ey8PThlNAIgwMCDp5WTB
DmFoRWTU6CpKtwIg/lb1ncbslH2xAFeUX6ASHXR8vBOnIXWss21FuAaNmWe4lmw=
=S+hs
```
-----END PGP PUBLIC KEY BLOCK-----
![image](https://github.com/user-attachments/assets/21cf095f-d221-48c1-8c9e-2737d76cf4de)

### Second Person
-----BEGIN PGP PUBLIC KEY BLOCK-----
Version: GnuPG v2.0.21 (MingW32)
```
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
=R5Hk
```
-----END PGP PUBLIC KEY BLOCK-----
![image](https://github.com/user-attachments/assets/7c42b1f2-1cee-4582-8a5f-09348b7304c4)

### Third Person
-----BEGIN PGP PUBLIC KEY BLOCK-----
Version: GnuPG v1
```
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
=qzaX
 ```
-----END PGP PUBLIC KEY BLOCK-----

![image](https://github.com/user-attachments/assets/2ade2de8-5c62-41e0-b115-87dea24aafb5)



## By searching on-line, what is an ASCII Armored Message?
An ASCII Armored Message, also known as "ASCII Armor" or "ASCII Armor Encoding," is a technique for converting binary data or non-textual information, like cryptographic keys or binary files, into text using only printable ASCII characters. ASCII (American Standard Code for Information Interchange) is a character encoding system that employs a 7-bit binary code to represent letters, numbers, and control characters.

This encoding ensures that the binary data can be transmitted or stored in text form without being altered or corrupted. It is especially useful when binary data must be included in text-based communication or storage, such as in emails or configuration files.

### Save the public key to your Ubuntu instance mykey.asc, and run:
```gpg mykey.asc ```
### What details can you get from the key
![image](https://github.com/user-attachments/assets/861b0bf3-52ab-4731-8d19-3b19814995ba)

## A.2 Bob has a private RSA key of:

 -----BEGIN RSA PRIVATE KEY-----
``` \nMIICXgIBAAKBgQDoIhiWs15X/6xiLAVcBzpgvnuvMzHBJk58wOWrdfyEAcTY10oG\n+6auNFGqQHYHbfKaZlEi4prAo
e01S/R6jpx8ZqJUN0WKNn5G9nmjJha9Pag28ftD\nrsT+4LktaQrxdNdrusP+qI0NiYbNBH6qvCrK0aGiucextehnuoqg
DcqmRwIDAQAB\nAoGAZCaJu0MJ2ieJxRU+/rRzoFeuXylUNwQC6toCfNY7quxkdDV2T8r038Xc0fpb\nsdrix3CLYuSnZ
aK3B76MbO/oXQVBjDQZ7jVQ5K41nVCEZOtRDBeX5Ue6CBs4iNmC\n+QyWx+u4OZPURq61YG7D+F1aWRvczdEZgKHPXl/+
s5pIvAkCQQDw4V6px/+DJuZV\n5Eg20OZe0m9Lvaq+G9UX2xTA2AUuH8Z79e+SCus6fMVl+Sf/W3y3uXp8B662bXhz\ny
heH67aDAkEA9rQrvmFj65n/D6eH4JAT4OP/+icQNgLYDW+u1Y+MdmD6A0YjehW3\nsuT9JH0rvEBET959kP0xCx+iFEjl
81tl7QJBAMcp4GZK2eXrxOjhnh/Mq51dKu6Z\n/NHBG3jlCIzGT8oqNaeK2jGLW6D5RxGgZ8TINR+HeVGR3JAzhTNftgM
JDtcCQQC3\nIqReXVmZaeXnrwu07f9zsI0zG5BzJ8VOpBt7OWah8fdmOsjXNgv55vbsAWdYBbUw\nPQ+lc+7WPRNKT5sz
/iM5AkEAi9Is+fgNy4q68nxPl1rBQUV3Bg3S7k7oCJ4+ju4W\nNXCCvRjQhpNVhlor7y4FC2p3thje9xox6QiwNr/5siy
ccw==\n-----END RSA PRIVATE KEY-----
 ```
And receives a ciphertext message of:
``` 
uW6FQth0pKaWc3haoqxbjIA7q2rF+G0Kx3z9ZDPZGU3NmBfzpD9ByU1ZBtbgKC8ATVZzwj15AeteOnbjO3EHQC4A5Nu0x
KTWpqpngYRGGmzMGtblW3wBlNQYovDsRUGt+cJK7RD0PKn6PMNqK5EQKCD6394K/gasQ9zA6fKn3f0=
```

Using the following code:
```
# https://asecuritysite.com/encryption/rsa_example
from Crypto.PublicKey import RSA
from Crypto.Cipher import PKCS1_OAEP
import base64
binPrivKey = "-----BEGIN RSA PRIVATE KEY-----
\nMIICXgIBAAKBgQDoIhiWs15X/6xiLAVcBzpgvnuvMzHBJk58wOWrdfyEAcTY10oG\n+6auNFGqQHYHbfKaZlEi4prAo
e01S/R6jpx8ZqJUN0WKNn5G9nmjJha9Pag28ftD\nrsT+4LktaQrxdNdrusP+qI0NiYbNBH6qvCrK0aGiucextehnuoqg
DcqmRwIDAQAB\nAoGAZCaJu0MJ2ieJxRU+/rRzoFeuXylUNwQC6toCfNY7quxkdDV2T8r038Xc0fpb\nsdrix3CLYuSnZ
aK3B76MbO/oXQVBjDQZ7jVQ5K41nVCEZOtRDBeX5Ue6CBs4iNmC\n+QyWx+u4OZPURq61YG7D+F1aWRvczdEZgKHPXl/+
s5pIvAkCQQDw4V6px/+DJuZV\n5Eg20OZe0m9Lvaq+G9UX2xTA2AUuH8Z79e+SCus6fMVl+Sf/W3y3uXp8B662bXhz\ny
heH67aDAkEA9rQrvmFj65n/D6eH4JAT4OP/+icQNgLYDW+u1Y+MdmD6A0YjehW3\nsuT9JH0rvEBET959kP0xCx+iFEjl
81tl7QJBAMcp4GZK2eXrxOjhnh/Mq51dKu6Z\n/NHBG3jlCIzGT8oqNaeK2jGLW6D5RxGgZ8TINR+HeVGR3JAzhTNftgM
JDtcCQQC3\nIqReXVmZaeXnrwu07f9zsI0zG5BzJ8VOpBt7OWah8fdmOsjXNgv55vbsAWdYBbUw\nPQ+lc+7WPRNKT5sz
/iM5AkEAi9Is+fgNy4q68nxPl1rBQUV3Bg3S7k7oCJ4+ju4W\nNXCCvRjQhpNVhlor7y4FC2p3thje9xox6QiwNr/5siy
ccw==\n-----END RSA PRIVATE KEY-----"
ciphertext=base64.b64decode("uW6FQth0pKaWc3haoqxbjIA7q2rF+G0Kx3z9ZDPZGU3NmBfzpD9ByU1ZBtbgKC8A
TVZzwj15AeteOnbjO3EHQC4A5Nu0xKTWpqpngYRGGmzMGtblW3wBlNQYovDsRUGt+cJK7RD0PKn6PMNqK5EQKCD6394K/
gasQ9zA6fKn3f0=")
privKeyObj = RSA.importKey(binPrivKey)
cipher = PKCS1_OAEP.new(privKeyObj)
message = cipher.decrypt(ciphertext)
print
print ("====Decrypted===")
print ("Message:",message)
```

What is the plaintext message that Bob has been sent:

 ``` Message: b'Python is your friend' ```


## B OpenSSL (RSA) (1p)

We will use OpenSSL to perform the following:

| No  | Description                                                                                                   | Result                                        |
| --- | ------------------------------------------------------------------------------------------------------------- | --------------------------------------------- |
| B.1 | First we need to generate a key pair with: `openssl genrsa -out private.pem 1024`<br>This file contains both the public and the private key.                           | **What is the type of public key method used?**<br> `RSA`<br>**How long is the default key?**<br>Use the following command to view the keys:<br>`cat private.pem` |
| B.2 | Use the following command to view the output file: `cat private.pem`                                           | **What can be observed at the start and end of the file?** <br>At the beginning and end of the file, we can see the header and footer markers that define the boundaries of the private key. These markers are characteristic of the PEM (Privacy Enhanced Mail) format, which is commonly used to encode cryptographic objects such as private keys and certificates in a human-readable format.                  |
| B.3 | Next we view the RSA key pair: `openssl rsa -in private.pem -text`                                             | **Which are the attributes of the key shown?** The private key consists of several key components: <br>- **Modulus (n)**: A large number, 1024 bits long, which is part of the RSA key. <br>- **Public Exponent (e)**: The public exponent, typically 65537 (0x10001). <br>- **Private Exponent (d)**: Used in RSA decryption. <br>- **Prime1 and Prime2**: The two prime numbers used to calculate the modulus (n). <br>- **Exponent1 and Exponent2**: Values related to the Chinese Remainder Theorem (CRT) optimization in RSA. <br>- **Coefficient**: Another component used in the CRT optimization. <br>Although Prime1, Prime2, Exponent1, Exponent2, and the Coefficient are not explicitly shown in the output, they are essential attributes of the private key <br>**What is the number of bits in the public modulus?**<br> 1024<br>**How many bits do the prime numbers have?**<br>512<br>**What is the value of `e`?**<br>65537(0x10001) |
| B.4 | Let's now secure the encrypted key with 128-bit AES: `openssl rsa -in private.pem -aes128 -out key3des.pem`     | **Why should you have a password on the usage of your private key?**<br>AES-128 is a symmetric encryption algorithm that facilitates the encryption and decryption of data. In this instance, it is specifically employed to encrypt the private key to safeguard it from unauthorized access. The password serves as an extra layer of security, acting as an encryption key that protects the private key.          |
| B.5 | Next, we will export the public key: `openssl rsa -in private.pem -out public.pem -outform PEM -pubout`        | **View the output key. What does the header and footer of the file identify?**<br>-----BEGIN PUBLIC KEY----- And-----END PUBLIC KEY---- |

## C OpenSSL (ECC) (1p)

Elliptic Curve Cryptography (ECC) is now used extensively within public key signing and key exchange, including with Bitcoin, Ethereum, Tor, and IoT applications. In this part of the lab, we will use OpenSSL to create an EC key pair. We will generate a random 256-bit private key (priv) and then generate a public key point (which is priv multiplied by G). This uses a generator point (G), which is an (x, y) point on the selected elliptic curve.

## C OpenSSL (ECC)

| No  | Description                                                                                                   | Result                                        |
| --- | ------------------------------------------------------------------------------------------------------------- | --------------------------------------------- |
| C.1 | First we need to generate a private key with:<br> ```bash<br> openssl ecparam -name secp256k1 -genkey -out priv.pem<br> ```<br> The file will only contain the private key, as we can generate the public key from this private key.<br> Now use `cat priv.pem` to view your key. | **Can you view your key?**<br> `Yes` 
| C.2 | We can view the details of the ECC parameters used with:<br> ```bash<br> openssl ecparam -in priv.pem -text -param_enc explicit -noout<br> ``` | Outline these values:<br> **- Prime (last two bytes):**<br> - A: 0 <br> - B: 7(0x7 )<br> **- Generator (last two bytes):** 0xb8, 184 in decimal<br> **- Order (last two bytes):0x41, 65 in decimal**|
| C.3 | Now generate your public key based on your private key with:<br> ```bash<br> openssl ec -in priv.pem -text -noout<br> ``` | **How many bits and bytes does your private key have?**<br>256 bits and 32 bytes<br> **How many bits and bytes does your public key have (Note the `04` is not part of the elliptic curve point)?** <br>64 bytes (512 bits)excluding 04<br> **What is the ECC method that you have used?**<br> The ECC (Elliptic Curve Cryptography) method used in the key is "secp256k1," a specific elliptic curve commonly employed in cryptocurrencies like Bitcoin, valued for its efficiency and security in cryptographic operations.|
| C.4 | First we need to generate a private key with:<br> ```bash<br> openssl ecparam -list_curves<br> ``` | **Outline three curves supported:**<br>secp256k1: Commonly used in cryptocurrencies like Bitcoin, this curve is defined over a 256-bit prime field and is known for its efficiency in blockchain technology.<br>secp384r1: Defined by both NIST and SECG, it operates over a 384-bit prime field, providing a higher level of security due to its larger key size. It is used in various cryptographic applications.<br>prime256v1 (P-256 or secp256r1): Defined by several standards bodies, it is widely used in SSL/TLS for secure communication over the internet and operates over a 256-bit prime field. |
| C.5 | Let's select two other curves:<br> ```bash<br> openssl ecparam -name secp128r1 -genkey -out priv.pem<br> openssl ecparam -in priv.pem -text -param_enc explicit -noout<br> openssl ecparam -name secp521r1 -genkey -out priv.pem<br> openssl ecparam -in priv.pem -text -param_enc explicit -noout<br> ``` | **How do `secp128r1`, `secp256k1`, and `secp521r1` differ in the parameters used?<br> Perhaps identify the length of the prime number used, and the size of the base point \( G \) and the prime number.How does the name of the curve relate to the prime number size?** <br>The key differences between the curves secp128k1, secp256k1, and secp521r1 lie in their field size (prime number size), coefficients, base point (G), and prime order (n). The field size directly corresponds to the name of the curve, with secp128k1 using a 128-bit field, secp256k1 using a 256-bit field, and secp521r1 using a 521-bit field. Larger prime numbers provide higher security, but require more computational resources. The base point G and prime order n differ in each curve, with secp521r1 offering the highest security due to its larger field size, while secp256k1 is commonly used in blockchain technologies like Bitcoin due to its efficiency.  |

## D. Elliptic Curve Encryption (1p)

In this example, Bob and Alice create elliptic curve key pairs. Bob can encrypt a message for Alice with her public key, and she can decrypt it using her private key. The following code demonstrates this process:

### Code Example:

```python
from cryptography.hazmat.primitives.asymmetric import ec
from cryptography.hazmat.primitives import serialization
import binascii
import sys

# Generate a private key using SECP256K1 elliptic curve
private_key = ec.generate_private_key(ec.SECP256K1())

# Extract and display the private key details
vals = private_key.private_numbers()
no_bits = vals.private_value.bit_length()
print(f"Private key value: {vals.private_value}. Number of bits: {no_bits}")

# Generate the public key based on the private key
public_key = private_key.public_key()
vals = public_key.public_numbers()
enc_point = binascii.b2a_hex(vals.encode_point()).decode()

# Display the public key in encoded point format
print(f"\nPublic key encoded point: {enc_point}")
print(f"x={enc_point[2:(len(enc_point)-2)//2+2]}")
print(f"y={enc_point[(len(enc_point)-2)//2+2:]}")

# Serialize the private key in PEM and DER formats
pem = private_key.private_bytes(
    encoding=serialization.Encoding.PEM,
    format=serialization.PrivateFormat.PKCS8,
    encryption_algorithm=serialization.NoEncryption()
)

der = private_key.private_bytes(
    encoding=serialization.Encoding.DER,
    format=serialization.PrivateFormat.PKCS8,
    encryption_algorithm=serialization.NoEncryption()
)

# Display the private key in PEM and DER formats
print("\nPrivate key (PEM):\n", pem.decode())
print("Private key (DER):\n", binascii.b2a_hex(der))

# Serialize the public key in PEM and DER formats
pem = public_key.public_bytes(
    encoding=serialization.Encoding.PEM,
    format=serialization.PublicFormat.SubjectPublicKeyInfo
)

der = public_key.public_bytes(
    encoding=serialization.Encoding.DER,
    format=serialization.PublicFormat.SubjectPublicKeyInfo
)

# Display the public key in PEM and DER formats
print("\nPublic key (PEM):\n", pem.decode())
print("Public key (DER):\n", binascii.b2a_hex(der))

```
```
Verify that the program runs, and observe the difference between the size of the public key
and the private key:
Private key size: 253 bits <br>
Public key size (in hexadecimal format): 512 bits
As observed, the public key is significantly larger in bits compared to the private key. This is typical in elliptic curve cryptographic systems, where the public key contains additional information that allows for signature verification and other cryptographic calculations. In contrast, the private key is smaller as it is only used to generate signatures and does not need to contain extra information.
```

### D.2 Let’s say we create an elliptic curve with y^2 = x^3 + 7, and with a prime number of 89 (y^2 = x^3 + 7 (mod 89)), generate the first five (x,y) points for the finite field elliptic curve. You can use the Python code at the following to generate them. https://asecuritysite.com/encryption/ecc_points_real (or for simpler code you can use https://asecuritysite.com/encryption/ecc_points3)
```
First five points:
(1, 39), (1, 50), (3, 52), (3, 37), (4, 31)
```

## E RSA

### E.1 A simple RSA program to encrypt and decrypt with RSA is given next. Prove its operation
``` python 
import rsa
(bob_pub, bob_priv) = rsa.newkeys(512)
7
msg='Here is my message'
ciphertext = rsa.encrypt(msg.encode(), bob_pub)
message = rsa.decrypt(ciphertext, bob_priv)
print(message.decode('utf8'))
```
Now add the lines following lines after the creation of the keys:

``` python
print (bob_pub)
print (bob_priv)
```

```
Can you identify what each of the elements of the public key (e,N), the private key (d,N), and 
the two prime number (p and q) are (if the numbers are long, just add the first few numbers of 
the value):
(e, N): Exponent e: 65537 AND Modulus N: 732417632585360785719009700...
• Private Exponent d: 65537
• Modulus N: 73241763258536078571900...
• First Prime Number p: 53416185642739962883…
• Second Prime Number q: 69830779611859413010…

When you identity the two prime numbers (p and q), with Python, can you prove that when 
they are multiplied together they result in the modulus value (N):
```
```
P * q es igual a N? True
Proven YES
```
### E.2  We will follow a basic RSA process. If you are struggling here, have a look at thefollowing page:

https://asecuritysite.com/encryption/rsa
First, pick two prime numbers:

```
p=2
q=7
```
Now calculate N (p.q) and PHI [(p-1).(q-1)]:
```
N= 14
PHI= 6
```
Now pick a value of e which does not share a factor with PHI [gcd(PHI,e)=1]:

``` e=5 ```

Now select a value of d, so that (e.d) (mod PHI) = 1
``` d=5 ```

Now for a message of M=5, calculate the cipher as:
```  C = Me(mod N) = 5^5(mod 14) = 3 ```

Now decrypt your ciphertext with:
``` M = 5 ```

Did you get the value of your message back (M=5)? If not, you have made a mistake, so go back and check. Now run the following code and prove that the decrypted cipher is the same as the message:

```python
import libnum
p=11
q=3
N=p*q
PHI=(p-1)*(q-1)
e=3
d= libnum.invmod(e,PHI)
print (e,N)
print (d,N)
M=4
print ("\nMessage:",M)
cipher = M**e % N
print ("Cipher:",cipher)
message = cipher**d % N
print ("Message:",message)
```
```
Select three more examples with different values of p and q, and then select e in order to 
make sure that the cipher will work:
```
![image](https://github.com/user-attachments/assets/e2aede3d-3108-46ad-b7e9-0b29ba51f450) ![image](https://github.com/user-attachments/assets/205f7113-0055-40ac-b767-91587170ff1c)  ![image](https://github.com/user-attachments/assets/a03fc521-6ada-4048-a464-3895a330abc0)


### E.3 In the RSA method, we have a value of e, and then determine d from (d.e) (modPHI)=1. But how do we use code to determine d? Well we can use the Euclideanalgorithm. The code for this is given at:

https://asecuritysite.com/encryption/inversemod

Using the code, can you determine the following:

```
Inverse of 53 (mod 120) = 77
Inverse of 65537 (mod 1034776851837418226012406113933120080) = 568411228254986589811047501435713
```

![image](https://github.com/user-attachments/assets/cb16948b-ab2e-4735-806f-0ff7ead68e3a)

### E.3 Run the following code and observe the output of the keys. If you now change the key generation key from ‘PEM’ to ‘DER’, how does the output change:

```python
from Crypto.PublicKey import RSA
key = RSA.generate(2048)
binPrivKey = key.exportKey('PEM')
binPubKey = key.publickey().exportKey('PEM')
print (binPrivKey)
print (binPubKey)
```
The main difference between DER and PEM formats is their encoding. DER is a binary format, more compact and suited for machine-readable data, without headers or footers. PEM is a text-based format, with base64-encoded content and headers/footer lines.

## F PGP(1p)
### F.1  The following is a PGP key pair. Using https://asecuritysite.com/encryption/pgp, can you determine the owner of the keys (or use gpg mykey.key):

```
-----BEGIN PGP PUBLIC KEY BLOCK-----
Version: OpenPGP.js v4.4.5
Comment: https://openpgpjs.org
xk0EXEOYvQECAIpLP8wfLxzgcolMpwgzcUzTlH0icggOIyuQKsHM4XNPugzU
X0NeaawrJhfi+f8hDRojJ5Fv8jBI0m/KwFMNTT8AEQEAAc0UYmlsbCA8Ymls
bEBob21lLmNvbT7CdQQQAQgAHwUCXEOYvQYLCQcIAwIEFQgKAgMWAgECGQEC
GwMCHgEACgkQoNsXEDYt2ZjkTAH/b6+pDfQLi6zg/Y0tHS5PPRv1323cwoay
vMcPjnWq+VfiNyXzY+UJKR1PXskzDvHMLOyVpUcjle5ChyT5LOw/ZM5NBFxD
mL0BAgDYlTsT06vVQxu3jmfLzKMAr4kLqqIuFFRCapRuHYLOjw1gJZS9p0bF
S0qS8zMEGpN9QZxkG8YEcH3gHxlrvALtABEBAAHCXwQYAQgACQUCXEOYvQIb
DAAKCRCg2xcQNi3ZmMAGAf9w/XazfELDG1W35l2zw12rKwM7rK97aFrtxz5W
XwA/5gqoVP0iQxklb9qpX7RVd6rLKu7zoX7F+sQod1sCWrMw
=cXT5
-----END PGP PUBLIC KEY BLOCK-----
-----BEGIN PGP PRIVATE KEY BLOCK-----
Version: OpenPGP.js v4.4.5
Comment: https://openpgpjs.org
xcBmBFxDmL0BAgCKSz/MHy8c4HKJTKcIM3FM05R9InIIDiMrkCrBzOFzT7oM
1F9DXmmsKyYX4vn/IQ0aIyeRb/IwSNJvysBTDU0/ABEBAAH+CQMIBNTT/OPv
TJzgvF+fLOsLsNYP64QfNHav5O744y0MLV/EZT3gsBwO9v4XF2SsZj6+EHbk
O9gWi31BAIDgSaDsJYf7xPOhp8iEWWwrUkC+jlGpdTsGDJpeYMIsVVv8Ycam
0g7MSRsL+dYQauIgtVb3dloLMPtuL59nVAYuIgD8HXyaH2vsEgSZSQn0kfvF
+dWeqJxwFM/uX5PVKcuYsroJFBEO1zas4ERfxbbwnsQgNHpjdIpueHx6/4EO
b1kmhOd6UT7BamubY7bcma1PBSv8PH31Jt8SzRRiaWxsIDxiaWxsQGhvbWUu
Y29tPsJ1BBABCAAfBQJcQ5i9BgsJBwgDAgQVCAoCAxYCAQIZAQIbAwIeAQAK
CRCg2xcQNi3ZmORMAf9vr6kN9AuLrOD9jS0dLk89G/XfbdzChrK8xw+Odar5
V+I3JfNj5QkpHU9eyTMO8cws7JWlRyOV7kKHJPks7D9kx8BmBFxDmL0BAgDY
lTsT06vVQxu3jmfLzKMAr4kLqqIuFFRCapRuHYLOjw1gJZS9p0bFS0qS8zME
GpN9QZxkG8YEcH3gHxlrvALtABEBAAH+CQMI2Gyk+BqVOgzgZX3C80JRLBRM
T4sLCHOUGlwaspe+qatOVjeEuxA5DuSs0bVMrw7mJYQZLtjNkFAT92lSwfxY
gavS/bILlw3QGA0CT5mqijKr0nurKkekKBDSGjkjVbIoPLMYHfepPOju1322
Nw4V3JQO4LBh/sdgGbRnwW3LhHEK4Qe70cuiert8C+S5xfG+T5RWADi5HR8u
UTyH8x1h0ZrOF7K0Wq4UcNvrUm6c35H6lClC4Zaar4JSN8fZPqVKLlHTVcL9
lpDzXxqxKjS05KXXZBh5wl8EGAEIAAkFAlxDmL0CGwwACgkQoNsXEDYt2ZjA
BgH/cP12s3xCwxtVt+Zds8NdqysDO6yve2ha7cc+Vl8AP+YKqFT9IkMZJW/a
qV+0VXeqyyru86F+xfrEKHdbAlqzMA==
=5NaF
-----END PGP PRIVATE KEY BLOCK-----
```
```
Owner is bill: <bill@home.com> 
```

### F.2 Using the Node.js code at the following link, generate a key:
https://asecuritysite.com/encryption/openpgp
Note: to add opengpg, you can install the required library with:
``` npm install openpgp ```
```
-----BEGIN PGP PUBLIC KEY BLOCK-----
Version: OpenPGP.js v4.10.10
Comment: https://openpgpjs.org
xk0EZSNWRQECAN0/s+5JBaRXGhzBWrkWAdOHqCRJRkWmwQda5kfXbKmZntQw
XlsJsRA+Fkb5YvqR1tiMc0R0WHba+n3AFv8uqYEAEQEAAc0UYmlsbCA8Ymls
24
bEBob21lLmNvbT7CjQQQAQgAIAUCZSNWRQYLCQcIAwIEFQgKAgQWAgEAAhkB
AhsDAh4BACEJEBmNmSDun6/BFiEEpm85dEqei3uJtfOoGY2ZIO6fr8Eb4QH/
UuDxEX3YbzPAMQPHaByE0ZdnzsY6R55upm8rvm2k6S4qhPDRkKADqKVNoz2F
DMWge0CFY+g9xXyWJ5AzCwJLuM5NBGUjVkUBAgCsu7bBZmj0B86aYY5rbWWc
YE/S5lslGO31P2sSywslcSdssLYxbLxULYC3m2Q46TRE9lE6MVU0Zxmd6Uvt
vsz/ABEBAAHCdgQYAQgACQUCZSNWRQIbDAAhCRAZjZkg7p+vwRYhBKZvOXRK
not7ibXzqBmNmSDun6/BaZ8B/0yta7ukCqjLOLV6XiBZbghbqrNLl9mE8aAU
HLcAAw4HY4uItsI8KneA+yw+O6xVjfvNzCZBbZH9mQtfDsqe4hU=
=nZYr
-----END PGP PUBLIC KEY BLOCK-----
```
```
-----BEGIN PGP PRIVATE KEY BLOCK-----
Version: OpenPGP.js v4.10.10
Comment: https://openpgpjs.org
xcBmBGUjVkUBAgDdP7PuSQWkVxocwVq5FgHTh6gkSUZFpsEHWuZH12ypmZ7U
MF5bCbEQPhZG+WL6kdbYjHNEdFh22vp9wBb/LqmBABEBAAH+CQMIRU6eehxz
EfbghrKbsn8iCbFLuVsJPM3rJ2QV0IyApMbLR/82o/9d8e86UpUhnpRUwUZ1
znQwXTvYz+fTBStZqo53tCrs+wj/eAL51r4LvhOm1aWhfW4KpJdbk8RqW2OY
QRZgf6aC3bX8vFOBypi00oBHGxHYfyXulNl9K3t3deNskzlrZayseECp5J1T
RyJq1ahxex1DDXzhHvobjjEkgf4AJExATa8ax2qS6RPxvbDqk22yVE0p9LC7
cS87Medj6qW/bPVf1eKVyMXE8VeWx3UifgFhzRRiaWxsIDxiaWxsQGhvbWUu
Y29tPsKNBBABCAAgBQJlI1ZFBgsJBwgDAgQVCAoCBBYCAQACGQECGwMCHgEA
IQkQGY2ZIO6fr8EWIQSmbzl0Sp6Le4m186gZjZkg7p+vwRvhAf9S4PERfdhv
M8AxA8doHITRl2fOxjpHnm6mbyu+baTpLiqE8NGQoAOopU2jPYUMxaB7QIVj
6D3FfJYnkDMLAku4x8BmBGUjVkUBAgCsu7bBZmj0B86aYY5rbWWcYE/S5lsl
GO31P2sSywslcSdssLYxbLxULYC3m2Q46TRE9lE6MVU0Zxmd6Uvtvsz/ABEB
AAH+CQMIhBwfbrjEpj/gNlxfKOVARE4zSIlFvKlOeL9E2XSeyS3homgsojVO
bv9S58RQ2FzeRtCnwTZVJXCWfAK3lFYKnHBmsDMXvgIP8dcA4FE9EPsZQy3+
rGCLtSk2H005Poi/ZlMtMpUomyggrfCo3lHDgFpqe/R28MOPkCeJJO+oAnZg
ZsnAb+d5EUf273uS56Gd0dCKJSxdei533XQiPIvIhLizIW90GATMVxK7W6ai
zetWA5y8Kbvlro7W4wMK9B+HdulxXb3d8Q1Ivks1FKb9SQJn0Lm5wnYEGAEI
AAkFAmUjVkUCGwwAIQkQGY2ZIO6fr8EWIQSmbzl0Sp6Le4m186gZjZkg7p+v
wWmfAf9MrWu7pAqoyzi1el4gWW4IW6qzS5fZhPGgFBy3AAMOB2OLiLbCPCp3
gPssPjusVY37zcwmQW2R/ZkLXw7KnuIV
=94uQ
-----END PGP PRIVATE KEY BLOCK-----
```
### F.3 An important element in data loss prevention is encrypted emails. In this part of the lab we will use an open source standard: PGP.
In this challenge, you should install a random number generator on your system with:
```sudo apt-get install rng-tools ```
| No  | Description | Result |
| --- | ----------- | ------ |
| 1   | - Create a key pair with (RSA and 2,048-bit keys):<br> `gpg --gen-key`<br> Now export your public key using the command:<br> `gpg --export -a "Your name" > mypub.key`<br> Now export your private key using the command:<br> `gpg --export-secret-key -a "Your name" > mipriv.key` | - How is the randomness generated?<br> - Outline the contents of your key file: |
| 2   | - Now send your lab partner your public key in the contents of an email, and ask them to import it onto their key ring (if you are doing this on your own, create another set of keys to simulate another user, or use Bill's public key - which is defined at [http://asecuritysite.com/public.txt](http://asecuritysite.com/public.txt) and send the email to him):<br> `gpg --import theirpublickey.key`<br> Now list your keys with:<br> `gpg --list-keys` | - Which keys are stored on your key ring and what details do they have: |
| 3   | - Create a text file, and save it. Next, encrypt the file with their public key:<br> `gpg -e -a -u "Your Name" -r "Your Lab Partner Name" he11o.txt` | - What does the `-a` option do?<br> - What does the `-r` option do?<br> - What does the `-u` option do?<br> - Which file does it produce and outline the format of its contents: |
|4|Send your encrypted file in an email to your lab partner, and get one back from them.<br>Now create a file (such as myfile.asc) and decrypt the email using the public key received from them with:<br>gpg –d myfile.asc > myfile.txt|Can you decrypt the message:|

















