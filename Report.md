# DM 103348: PROJECT: RSA-CRYPTOGRAPHY MESSAGE ENCODER & DECODER WITH USER PROVIDED KEY #

### PROJECT MEMBERS ###
 - **64299** | **Hafiz Daniyal Shakeel**
 - 64359 | Syed Shaan Ali Rizvi
 - 64239 | Syed Muhammad Uzair 
 - 64335 | Syeda Raahima Batool Zaidi 
 - 63372 | Rabbiya Mehmood

## Project Description ##
we have design a project to implement a message encryption-decryption application according to the Vigenere cipher, which can encrypt the message using the key and can decrypt the encrypted hash using same key(Symmetric).

## Discrete Math Concepts Used ##
We used Modulo arthimetic and ciphers to implement encryption and decryprtion.
### Example 1: Encode/Encryption ### 
```python
def encode(self):
		enc = [] 
		msg=self.txtm.text()
		key=self.txtk.text()
		for i in range(len(msg)): 
			key_c = key[i % len(key)] 
			enc_c = chr((ord(msg[i]) + ord(key_c)) % 256)
			enc.append(enc_c) 
		self.lbem.append(base64.urlsafe_b64encode("".join(enc).encode()).decode()) 
```

## Problems Faced ##
We haven't face that much problem.
