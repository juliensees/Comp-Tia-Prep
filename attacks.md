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

### Network and App Attacks

- On-path attack - when an attacker is between two targets communications
        - formerly "man-in-the-middle"

      - DNS Poisoning - an attack agains the DNS system that resolves a requeset away from legitimate                servers  
              * DNS IS THE SYSTEM THAT RETURNS AN IP ADDRESS FROM A GIVEN DOMAIN NAME  
             - Domains that host malware then have a negative reputation
      
     - ARP Poisoning - when an attacker changes Address Resolution Protocol (ARP) records in a way that                     resolves the attacker's MAC address to a legitimate IP address
 
- App Attacks

   * Resource exhaustion attacks    
     - Denial-of-service (DoS)    
             - where an attacker attempts to make a networked resource unavailable to others by                                disrupting and overwhelming. 
     - Distributed-Denial-of-Service (DDoS)    
             - a DoS attack in which multiple computers work together to cause a denial of service. 
             - the attacking computers are usually compromised by malicious software. 
     - DNS Amplification attack.  
             - when an attacker spoofs lookup requests to DNS servers and redirects the response  
                toward a target. 
                  - the response is larger than the request, allowing the attacker to amplify efforts
      - Buffer overflow. 
              - when a program overruns a buffer's boundary as a result of a too-large input and.                                overwrites adjacent memory locations. 
                 - memory locations are often well-defined, allowing an attacker to write the overflow.                          code into an executable area of the memory
                    
              * can be used to change info and escalate privileges 
        - Privilege escalation
                - when an attacker elevates his privileges to gain access to resources he wouldnt have
                - the ability to elevate the privileges can be caused by a bug or simple oversight
