# asym_encryption
A few assignments were I learn about asymmetric encryption  

Opgave 1
Funcities voor asymmetrische encryptie: openssl_pkey_get_public, openssl_public_encrypt, openssl_get_privatekey, openssl_private_decrypt

Opgave 2
Het is afhankelijk van padding hoeveelheid bits die RSA key heeft. Bijvoorbeeld met OAEP RSA-key met 1024 bits kan 86 bytes encrypten. RSA key met 2048 bits kan 214 bytes encrypten.

Opgave 3
SSH key gebruik je voor connectie tussen je IntelliJ en Github aanmaken om version control secure en zonder nodige inlog doorsturen. IntelliJ genereert de SSH-key maar je moet ze wel op je Github vastzetten om voor connectie te zorgen. 

Opgave 4
  1 - Bob moet public key van Alice krijgen. Dan die word gebruikt om session-key van Bob te encrypten en doorsturen naar Alice. Als Alice de session-key van Bob heeft dan kan ze die gebruiken om andere berichten van Bob te decrypten.
  
  2 - Als Alice wilt berichten van bob decrypten moet ze eerst hem een Public Key sturen. Dan krijgt ze een bericht die moet ze decrypten met ze private key, daarin zit de session-key. Die gaat ze gebruiken om rest van de berichten de decrypten.
