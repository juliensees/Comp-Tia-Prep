Hashing  
  - one way... can't go back  
  - used to ensure integrity and safeguard passwords  

  - creates a unique output (digest) from a given input  
  - Collision - when two different inputs yield the same output  
      - if this happens, the hashing algorithm is considered broken  
   
  - mostly use sha256, or even sha512sum (even longer hash)... md5 is old, less secure, and rarely used  



Encryption
  - two-way... can encrypt and decrypt  
  - used to ensure confidentiality   

  - Symmetric  
      - the encoding key is the same as the decoding key  
      - ROT13 cipher - just shifts the alphabet by 13, so A is N, etc.  
        - can be easily broken by brute force and/or frequency analysis    
      - THE KEY NEEDS TO BE SHARED... HOW DO YOU DO THAT?  
        --- this is the issue with symmetric keys  
      - less computationally intense... uses a lot of computing power/time/energy  
   
  - Asymmetric  
      - thousands of digits long... very computationally intense   
      - utilizes a public and private key  
      - OFTEN USE ASYMMETRIC TO ESTABLISH A LINK, AND THEN USE SYMMETRIC TO CONTINUE COMMUNICATION  

      +  In-band Exchange - when keys are exchanged over the same channel... like the public key  
      +  Out-of-band Exchange - when keys are sent over an unrelated channel  
            - ex. relaying a key verbally or sending it in the mail  
                - has the possibility of infiltration/comprimised
             
  - PKI and Certificates  
      - PKI (Public Key Infrastructure)  
            - public key infrastructure ensures a public key belongs to only one organization  
              - ISSUED BY A CA (Certificate Authority)  
              - OR SELF-SIGNED BY YOUR ORGANIZATION ----- WON'T GO OUT ONTO THE INTERNET  
          - CA will check if key pair is unique, and assigns a key pair for a length of time  
               - maintains records of assigned certificates  
               - trusted because authority was granted by another CA in a heirarchy  

        - OCSP (Online Certificate Status Protocol) - allows entity to check status of certificate  
        - CRL (Certificate Revocation List) - identifies which certificates have been revoked by the                         issuing CA and shouldn't be trusted  
        
