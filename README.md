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
mQINBFIpG2IBEACuiDv9Lo8UW0eUh9sUvB11tncGMIgJczcdSlHXNoApf0uEmTPw
ngIpmkeOdXniLeEHv2eao98I3IjtIfvo2YfnqFQ2lSn+UUfnCf+nh6jYAnyEOCIi
dr8oXN5Lx91XfRCdU17oGYW6azTIKZqxLQticf0GvCaXYHdBaAqU5E1C20sC6CnV
IlqIxr/kjzvQdhZ1Ig8LPu9Ol7ltsf6BevEI0wSLJFRZXF3mHb9iYNtJnz+gWj/S
XBWcgJpFblH0dOo8gyF/K58HBMh8NPo9nQqO9bWmo/TMPzdX5DERGMaZ92tg34I6
bFjGj2oflu22o8WlOZn07iXAkJKG6BLcnOT4tpqVCWrM2YBr+eD7BR9Q2qRaJQ3T
8fm2ohYHiLjqkvH7/LjpGTilcdwkHmUjr9pD/MJQZR5BsyyWg0a6A35jvViAVaAo
Zkz+wFE6TCIdPGBj9q+vH++F3MZDl/qREiWeUn1cu01JobPJIr6b48eyLkxHbeu3
z1GlIuzNfC8al/Wr9rPJZpOehf/woddIdkxnYvqyyxXo/t7/7ksMJglW6VVVKVgG
mWEFHoL93pcKXZdqImsCUtK362v8qrb3RlhG/zgFHBRljcvAVbeP+Y7HayeO756i
WewGiy/9Z5dlS1MV594fhXM9BzwMWfbosZBivi1jvOEyTSpma3q0fHx/tQARAQAB
tCBzY2huZWllciA8c2NobmVpZXJAc2NobmVpZXIuY29tPokCOQQTAQIAIwUCUikb
YgIbAwcLCQgHAwIBBhUIAgkKCwQWAgMBAh4BAheAAAoJELS0KiztrOpnODkP/3PA
sx0r2/6D48GLqTmUBwJiK6z4EmNaMmwElvqzeadc7DknzSqHKWDcDCZPxllIlDRv
kdAx7kKq+zuSAfzEtK+KZ4jm0ahn5bpdDzp+j8YHvym+JXcmy+JSIgdtQmCybT0B
1xPyrVpxK7uEr6M+XBxIZ8OfpKf1uQbBQllwL47ejgYGdHP5kX0dMb2hr4OcfpxC
ah/OXf3CpXYuOxrFIQ+b0NoqQCcap/6ggVO/cKO06d9J+xhJd0Rv5B4ILBLx0/PM
Y4UbOs/7uAOwTkQTCIUkURq2mIHQBy4jLIVaOACdwHaKaC6C6Q6/rSiNHDQuOKZF
Q0LVS+ygiQg7VWyA1dVsyGZTeIlQ6UwHARasrSs6AtKHbKaU6cZ1IKYmv+y5vQ3u
dfl2cePriJIJgiZEFWe/iH5tDvIQkGkUnOACvVMtMtP9tfhL6igrMazck/JjXRHv
RL1VUKwZx0rQrT7APxHBL/wAwCLE4Hf6eEMegyeqkY7l/bSTTvwGfA+VlMGyi93v
5J9JNopmk9XRCGjYlK1uDxSvWnJIm5BpQVGFFx0bLx+0Y89fVwqKzOuv5DvQ7CRT
EMuBSDZrZLpS0y7yBHfYHijxV3R7/LQvWr04uaAViPrTUFvHrY4vxDk43YHLjeQ8
Eu3SnlSp19cAVXiImAdd5kp7koG4+6k0zDHyla7puQINBFIpG2IBEAC48ibokoiU
+lIFRGWk1ZOHxGQXZkh9LRocpaUF+b0AonYjWD/tzoQ/KhMWU6aPiu/Ldg7FcdFY
o7FnCLkz1FMRhr3oS0YrkUiEirWGPEWMJdwrGp0t6ecy2g0Q0Jhc8O8JNE5pAmtE
tVkb2MWgD0hRUIoFSO/abtCtQUkV7ymkPNJ5HTArNjjCcZ9QdQZykAqYqXhKbv2W
IMe/tUGaJYFw5xpuMdZ+etm8xFuw6iLO5EgDtLvAp7yooqOgQIXwXG0EBMshFdqO
ivpgG/JldYqx1li2S53wiCqHXJr7M9Ch23Maix14/6Q6PK20KgLjeo9WTgLCJjB1
krUNbgbWOQIxk/ZgXcs4Z+VJXAFHrL3yoR+rBKYDDDjnSm0oWCvfYmNADSwaNPgJ
cLL4/ibTUZZBezMqppfyTZjrBI1Ng+UMoRyMeJe3Ypg6/HvQ82B6wPSZZs49YkKK
F36TrHUuSuO2vlVELb9NYM8ZVG8hJ/Og/PVyGKGCEb0EwgefwMomKRlNbk7IQoAb
fzbhhRlhyZbFAD3QtuCJnTyHb/FSoXGS/PDpRyFRMQQsNQznded5TzAqmbnw1ZAQ
zbZ/A3WKNoSrsyY97y8XZhXMlcpYOsUR7hGJoxQOizw57Y42nGltJpyntYGR/M10
0Xl+h0zrSfCwG86GZHhhgvG4I/RdgwvWVQARAQABiQIfBBgBAgAJBQJSKRtiAhsM
AAoJELS0KiztrOpn9ikP/i22bfoOzsyqG57YL2yxG2AM0N/qy5yfJT9uNJky3rRW
zZ+iEglOKKwCj60fKbp9snm3Xyj8t6LGrM6Qu8YuKX40wHx7m2VUpgheeKoZAHV2
9oCnwkJ8V3OJhp7D32O0TRya4ZhAXNrAGqEPUp0E8Yep/bWPUAlNtOxp1y2sJIHG
mtcEee0J/AFJvU3BS885IbJxCA3YdEbgx45B8Et74WpCj4LuWrii7GmEnXbh/kv/
JLzniZCV/5F/+8dfUZld/02GYZN02lorlbzdbZkkh6dc+GbyN0kSnQMEBhIp9xDW
RdtbHdJpMNUxZyFAhCU7k1bTs5Fo1QNgug76LQhlhSwc/DpZWMTeKwas7P8VelAu
5ZX3eUV0pB+sinFb+ArhW9nCtBBebLAJTL86tlxe4mq4C9sHV4AW6amcisAU8OEN
e2MX3zIbN9I23EM+5mRVfGHavVR0gRU8M/QcO9FEP5Q3nFt6rWWfYMPSwV0Vk1kG
ThswcgVlMG/ed6u2zlt4A39V414Lz/fECSFlTo1f3T3i2j06TT+QNMj/4jMZHsqj
QlRYkxLnN2DRwmbPJeBtGCfW3wvhDZJ0w1XvBcO9fJLIkw87swaFCQclw66EM2Ga
Mhc2jkLSMoXGEv/OHvneDPIZN9lSJWweHtVayhk2buFMxWka4sVTrfMvFx4Fm5ve
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
| C.2 | We can view the details of the ECC parameters used with:<br> ```bash<br> openssl ecparam -in priv.pem -text -param_enc explicit -noout<br> ``` | Outline these values:<br> **- Prime (last two bytes):**<br> - A: 0 <br> - B: 7(0x7 )<br> **- Generator (last two bytes):**0xb8, 184 in decimal<br> **- Order (last two bytes):0x41, 65 in decimal**|
| C.3 | Now generate your public key based on your private key with:<br> ```bash<br> openssl ec -in priv.pem -text -noout<br> ``` | **How many bits and bytes does your private key have?**<br>256 bits and 32 bytes<br> **How many bits and bytes does your public key have (Note the `04` is not part of the elliptic curve point)?** <br>64 bytes (512 bits)excluding 04<br> **What is the ECC method that you have used?**<br> The ECC (Elliptic Curve Cryptography) method used in the key is "secp256k1," a specific elliptic curve commonly employed in cryptocurrencies like Bitcoin, valued for its efficiency and security in cryptographic operations.|
| C.4 | First we need to generate a private key with:<br> ```bash<br> openssl ecparam -list_curves<br> ``` | **Outline three curves supported:**<br>secp256k1: Commonly used in cryptocurrencies like Bitcoin, this curve is defined over a 256-bit prime field and is known for its efficiency in blockchain technology.<br>secp384r1: Defined by both NIST and SECG, it operates over a 384-bit prime field, providing a higher level of security due to its larger key size. It is used in various cryptographic applications.<br>prime256v1 (P-256 or secp256r1): Defined by several standards bodies, it is widely used in SSL/TLS for secure communication over the internet and operates over a 256-bit prime field. |
| C.5 | Let's select two other curves:<br> ```bash<br> openssl ecparam -name secp128r1 -genkey -out priv.pem<br> openssl ecparam -in priv.pem -text -param_enc explicit -noout<br> openssl ecparam -name secp521r1 -genkey -out priv.pem<br> openssl ecparam -in priv.pem -text -param_enc explicit -noout<br> ``` | How do `secp128r1`, `secp256k1`, and `secp521r1` differ in the parameters used?<br> Perhaps identify the length of the prime number used, and the size of the base point \( G \) and the prime number.How does the name of the curve relate to the prime number size?<br>The key differences between the curves secp128k1, secp256k1, and secp521r1 lie in their field size (prime number size), coefficients, base point (G), and prime order (n). The field size directly corresponds to the name of the curve, with secp128k1 using a 128-bit field, secp256k1 using a 256-bit field, and secp521r1 using a 521-bit field. Larger prime numbers provide higher security, but require more computational resources. The base point G and prime order n differ in each curve, with secp521r1 offering the highest security due to its larger field size, while secp256k1 is commonly used in blockchain technologies like Bitcoin due to its efficiency.  |

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




