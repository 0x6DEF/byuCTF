# Take Me Out to the Ball Game - Writeup
### ===================================

### Challenge

>
>I like baseball, do you?? I think grand slams are the coolest!!!
>
>'16DLF592KN4KKI9BNJHCM179GML30PB32235B04MDM145GJD04N9NFL'
>


At first, I'm not good at baseball and i don't know the game rules

when i saw baseball i didn't know he meant base encoding i recently

discovered. 

but my solve way was that i took this hash and put it to

cyberchef and decoder.fr also i did the same with crackstation.net to

identify the hash but i got nothing so i moved to baseball game and i

searched for the game rules and the information began to intertwine

when i'm reading the rules i figured out that "A game is played out

between two teams, each made up of 9 players" and "The object of

baseball is to score more runs than your opponent. The idea is to hit

the ball thrown at you as far as you can before running around 4 bases

to complete a run" 

i really don't understand these words correctly but

i thought with hacker mindset challenge says "baseball" so it starts

with base for me i considered it for base encoding and while reading

about rules it says "each made up of 9 players" so i had to make sure

that cyberchef it not a stupid i got a base29 encoded and i put it to

cyberchef and nothing can't recognize it as decoder.fr so i made a python

script and i tested the fake one and it worked, i grabbed the

challenge encoded and put it and it worked too and returned the flag

:DD

![[base.png]]

```solve.py

# encoded

enc = "16DLF592KN4KKI9BNJHCM179GML30PB32235B04MDM145GJD04N9NFL"

  

# encoded base

base = int(enc, 29)

  

# convert to hex

convert_to_hex = hex(base)

  

# remove first two 0x from the hex

convert_to_hex = convert_to_hex[2:]

  
  

# convert to bytes then to string and print it

print(bytes.fromhex(convert_to_hex).decode("utf-8") )

# FLAG: byuctf{4ll_th3_b4s3s_4r3_10ad3d!}
```


Finally i got Take Me Out to the Ball Game Challenge