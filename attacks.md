### Cryptographic Attacks

* Password Attacks

    * Brute Force - attempting to guess a password by trying every combination. 
          - takes a long time. 
    * Dictionary Attack.  
          - trying a list of previously used possible passwords to guess. 
    * Password spraying  
          - trying one "known-good" password across many accounts. 
            - trying once, so no account lockouts or failed password timeouts. 

    * Birthday attack - statistical method to find a collision   
    * Collision attack - when two hashed inputs match, an attacker uses the collision that was found to.              figure out what the hash values are. 
    * Known plaintext attack. 
          - when an attacker has access to both the plaintext and ciphertext of an encryption method. 
            - they can then use this to decipher encrypted messages. 
    * Known ciphertext attack. 
          - attacker knows just the ciphertext... harder to find weaknesses  

    * Rainbow tables
          - a table of previously-computed values for reversing hashing functions
          - looks for patterns within hash values
            - attacker needs to know which hash algorithm was used

  ### Hardware Attacks

  Physical attacks

    - Malicious USB cables. 
        - can be loaded with scripts. 
    - Malicious flash drives. 
        - sometimes dropped purposely in a parking lot, hoping someone picks it up and brings it inside               building to inspect what's on it. 
     
          * both of these devices is Hak5 - they make pen testing tools
         
    - Card cloning. 
          - someone makes a copy of your RFID badge by just bumping against your RFID badge with their  
            reader
    - Skimming
          - special hardware that is inserted into an ATM or gas pump to steal PIN and card info
