# php_base64encrypted
Encrypt base64 via PHP. Short, fast, easy, practice and safe (-quantom aside ^_^- this encryption is impossible to break).

Example: 

Base64_Encrypted::Crypter("Hello World ! My nickname is Boby. Have fun.","My First Key","Anti Force Brute Second Key");
 
 and to decrypt:
 
Base64_Encrypted::Decrypter( "aQZ8978TaGBdg58RHgupAMDxMlHfexlSNxFoFhvF1A9gz8WLjUL+Qqvw2rHJCvAcoI4", "My First Key", "Anti Force Brute Second Key");

 
 To check the integrity of the encrypted data, add true to the fourth parameter.
 
Example:
 
Base64_Encrypted::Crypter("Hello World ! My nickname is Boby. Have fun.","My First Key","Anti Force Brute Second Key", true);

and to decrypt:

Base64_Encrypted::Decrypter( "1mL+b/gpbUuf9yH4SLLXxrmZn348rwdGFM5uktnZtGzPUE+eKCugEHyXrmvG24j4xtHtYSKJxTm","My First Key", "Anti Force Brute Second Key", true);


The "Paranoiac" mode allows to add two other passwords to annihilate any attempt of attack by brute force and without affecting performances:

Example:

Base64_Encrypted::Decrypter( "Hello World ! My nickname is Boby. Have fun.", "My First Key","Anti Force Brute Second Key", true, "Paranoiac Key 1", "Paranoiac Key 2");


and to decrypt:


Base64_Encrypted::Decrypter( "XkDcz64cU8KzYzASATaWqfWTCvpDerqmSKmjIBsDgZfznCXqHqdWgigqaR8tUmjYQmUBWyoxkjq", "My First Key","Anti Force Brute Second Key", true, "Paranoiac Key 1", "Paranoiac Key 2");





Ref: http://inseparables.j-ad.net/archives/24/

PS: Un big merci à Steph dit la fouine :) pour ses avis éclairés !
