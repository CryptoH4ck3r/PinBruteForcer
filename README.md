# Pin Brute Forcing Script  
  
*A simple for loop function that we can use to brute force a pin in our target.*  
  

Do you find yourself looking at a server that you need to discover a 4-Digit pin? Maybe it is a 6, or 8 digit pin that you need to crack? This brute forcing program will allow you to do just that!  
  
The basic structure of the code is as follows;  
  
```
#!/bin/bash  
  
passwordforuser=abc123  
  
  
for $i in {1111..9999}; do
        echo "$passwordforuser $i"
done | nc localhost 1234

```

Let's break this down just a little bit for us to understand how it works and how we can configure it.  
  
(#!/bin/bash) ~ Leave this alone! LOL  
  
(passwordforuser=abc123) ~ You can change the variable name {passwordforuser} if you desire, but you will need to change the echo command too. You can change the {abc123} to the password you want to use.  
  
(for $i in {1111..9999}; do ~ What we are doing, is calling a variable "i" and telling our script to check for every possible combination of Pins that we can use. I selected default 1111..9999. You can change these options to go bigger, smaller, more digits, or less. All up to you!  
  
(echo "$passwordforuser $i") ~ Here we have the output command that will echo the results of the password for the user, plus the pin that it generated for us automatically.  
  
(done | nc localhost 1234) ~ And we told the script it is done, however, we utilize netcat in order to connect to the localhost on port 1234. You can change "localhost" to your target's URL/IP, and you can change the port from 1234 to the one you need!  
  
## Please Note:  
*This script is for educational purposes only. Any illegal actions you take utilizing this tool is on you. I, CryptoH4ck3r, am not responsible for your actions!*  
  
## Connect with Crypto H4ck3r  
If you would like to connect with Crypto H4ck3r and talk about programming, hacking, or anything else, AWESOME! Let's connect here;  
**Email:** *cryptoh4ck3r@proton.me*  
**Twitter:** *https://www.twitter.com/CryptoH4ck3r*  
  
If you liked this script, and would like to see more come fromt he author, please help support them. They are running dangerously low on coffee!  
BitCoin Wallet (Recieving):  
3QVThxXUbV4uaKBBJP1bHahZH2iJhpmncT  
  
Etherum Wallet (Recieving):  
0x07a0d46097C63Ee7E66229821fc0115Bb0E2F424  
  
Doge Wallet (Recieving):  
DRjYNp9JGbkFSVL5tXQqbU6y8Wy99bJA8m  
