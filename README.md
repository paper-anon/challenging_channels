#  Challenging Channels
This repository contains keys, scripts and data utilized for the paper "Challenging Channels"


## CS
**challenger.py** provides four modes: legitimate symmetric (ls), legitimate asymmetric (la), covert symmetric (cs) and covert assymetric (ca). 
*change target IP*: To change the target IP (i.e. the challenger IP) edit the following line: soc.connect(("192.168.3.29",10001))

### ls
python3 prover.py ls <token logging file>

### la
python3 prover.py la <token logging file>

### cs
python3 prover.py cs <covert message file> <alphabet file> <token logging file>  <# of chars at once> 

### ca
python3 challenger.py ca <covert message file> <# of chars at once> <token logging file> 
  
*data*
 contains alphabets and scripts that were used in the paper. Please note that the malicious scripts are provided in an encrypted .zip file. 
  **Do not execute these scripts**. As these have been found in the wild and are clearly malicious and **will be detected by antivirus software**. 
  The password is "Virus"
  
  
  
**public_key_challenger.pem** public key of the challenger

**private_key_prover.pem** private key of the prover
  
  

## CR
**challenger.py** provides four modes: legitimate symmetric (ls), legitimate asymmetric (la), covert symmetric (cs) and covert assymetric (ca)
*change listening IP*: To change the listening IP (i.e. the challenger IP) edit the following line: soc.bind(("192.168.3.29",10001))
### ls
python3 challenger.py ls

### la
python3 challenger.py la

### cs
python3 challenger.py cs <alphabet file> <# of chars at once>

### ca
python3 challenger.py ca
  

  
  
**public_key_prover.pem** public key of the prover

**private_key_challenger.pem** private key of the challenger
