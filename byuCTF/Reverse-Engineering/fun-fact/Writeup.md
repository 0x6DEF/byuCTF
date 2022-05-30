# Fun Fact Writeup

- Easy


```fun-fact
This was an easy challenge to warm up xd they gave us a python file

called "obfuscated.py" has a base64 encoded string/real_script_code

once i decoded the base64 i got the script code readable there were 2

ways for me to solve this challenge but i choosed the easy way after i

ran it asked me to choose 1 option of 3 options: 

1- print the flag


2-Enter 2 for a fun fact about ocean creatures


3- Enter 3 to continue


of course first option not going to print the flag so i choosed the

third one to continue it asked for flag, and after reading the source

code i saw that it makes an equation and prints the user_input after

made this equation so i typed the encrypted string in the file:


encrypted = "".join([chr(ord(x) ^ ord(key)) for x in user_input])

print("encrypted: ", encrypted)

if(encrypted == 'g%4c$zc%dz4gg;'):


print("Success!") 

else:

print("\nTry again")



option_three()

- [ ] i typed it "g%4c$zc%dz4gg;" and it returned a string seems to be

a flag [ 0rc4s-4r3-c00l ] i tried it and it worked

```

![fun-fact](https://github.com/0x6DEF/byuCTF/blob/main/byuCTF/Reverse-Engineering/fun-fact/Pasted%20image%2020220529161444.png)

### FLAG: byuctf{0rc4s-4r3-c00l}

