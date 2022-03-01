#  Challenging Channels
This repository contains keys, scripts and data utilized for the paper "Challenging Channels"


## CS
*rules.sh* sets the iptables rules to catch packets from the os. The IP has to be changed to the OS-IP within the file

*forwarder_add_partial_cc.py* fetches hash-containing packets and modifies them if necessary. The file contains hard-coded target and source IPs, that have to be modified

Usage :`python3 forwarder_add_partial_cc.py <CC-share in percent - integer>`

*covertmessage.txt*: the message to encode

*alphabet.txt*: the alphabet to utilize

## CR
*challenger.py* provides four modes: legitimate symmetric (ls), legitimate asymmetric (la), covert symmetric (cs) and covert assymetric (ca)
Synthax is as follows for each mode:
### ls
python3 challenger.py ls

### la
python3 challenger.py la

### cs
python3 challenger.py cs <Alphabet File> <Number of Chars>

### ca
python3 challenger.py ca
  

*public_key_prover.pem* public key of the prover

*private_key_challenger.pem* private key of the challenger
