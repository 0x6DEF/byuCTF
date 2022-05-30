# Chicken - Writeup
#### =====================

### Challenge

```chicken

So I tried learning a new sorta-language, but I'm not very good at it and don't think I used it right. Can you check for me?


and chicken.chn file
```

![chickenwords.png](https://github.com/0x6DEF/byuCTF/blob/main/byuCTF/Reverse-Engineering/chicken/chickenwords.png)

   Opps, i don't know what is this chicken lol?..

   so google is my friend at this moment, after searching in different

   ways i found that chicken esolang known as

   (shockingly) [chicken](https://esolangs.org/wiki/Chicken).

   each line has the word "chicken" written a certain number of times.

   and that means when count the number of chicken on each line you will

   get a something called opcode Skip this part:

   i searched for tool that can translate those lines to me

   automatically and i found a tool on github:

   [GithubTool](https://github.com/kosayoda/chickenpy)

![tool](https://github.com/0x6DEF/byuCTF/blob/main/byuCTF/Reverse-Engineering/chicken/Capture.png)

  it translate the lines to be easier to read after i ran the tool and

  got the result was kinda easy to me to read it and arrange the flag
   <h3>Result:</h3>
```
chickenpy.VM - Storing 's' to 35

chickenpy.VM - Storing '3' to 15

chickenpy.VM - Storing '' to 12

chickenpy.VM - Storing 't' to 7

chickenpy.VM - Storing 'ˡ' to 24

chickenpy.VM - Storing '' to 36

chickenpy.VM - Storing 'e' to 19

chickenpy.VM - Storing '0' to 23

chickenpy.VM - Storing 'z' to 46

chickenpy.VM - Storing 'n' to 33

chickenpy.VM - Storing 'w' to 22

chickenpy.VM - Storing '3' to 17

chickenpy.VM - Storing '3' to 11

chickenpy.VM - Storing '' to 40

chickenpy.VM - Storing 'a' to 45

chickenpy.VM - Storing '0' to 30

chickenpy.VM - Storing 'f' to 5

chickenpy.VM - Storing 'r' to 14

chickenpy.VM - Storing 'l' to 31

chickenpy.VM - Storing 'n' to 20

chickenpy.VM - Storing '1' to 41

chickenpy.VM - Storing '3' to 9

chickenpy.VM - Storing '3' to 26

chickenpy.VM - Storing 'y' to 1

chickenpy.VM - Storing '4' to 13

chickenpy.VM - Storing 'c' to 3

chickenpy.VM - Storing '}' to 49

chickenpy.VM - Storing 's' to 29

chickenpy.VM - Storing 's' to 25

chickenpy.VM - Storing 'y' to 48

chickenpy.VM - Storing 'z' to 47

chickenpy.VM - Storing 'm' to 42

chickenpy.VM - Storing 't' to 4

chickenpy.VM - Storing '' to 27

chickenpy.VM - Storing 'r' to 10

chickenpy.VM - Storing 'h' to 8

chickenpy.VM - Storing 't' to 39

chickenpy.VM - Storing 'g' to 34

chickenpy.VM - Storing 'v' to 18

chickenpy.VM - Storing '' to 21

chickenpy.VM - Storing 'u' to 38

chickenpy.VM - Storing '' to 16

chickenpy.VM - Storing 'u' to 2

chickenpy.VM - Storing '_' to 43

chickenpy.VM - Storing '4' to 32

chickenpy.VM - Storing 'l' to 44

chickenpy.VM - Storing 'b' to 37

chickenpy.VM - Storing '{' to 6

chickenpy.VM - Storing 'e' to 28

chickenpy.VM - Storing 'b' to 0
```

 i noticed that every number

 represent a letter for example: storing 'u' to 38, index number 38

 is letter 'u' and storing 'b' to 0 , 'b' stored in index 0

 and so on, i started combining them started from index 0 to the last
 
 index that was 49 so since we start counting from 0 i'll see if 0 matches the letter 'b' cuz 
 
 the flag is always starts with letter "b" if yes i will keep going to letter y and if it matches 
 
 index 1 that means counting is right cuz next letter in the flag is y,

 once i done collected the flag

  [ byuctf{th3r3_4r3_3ven_w01s3_es0l4ngs_but_1m_lazzy} ]

 i submitted it and site said not valid, i asked the stuff they told me

 "w01s3" not a word so i thought to replace the numbers with their

 normal letters and translate it on google like this 
 {there_are_even_woise_esolengs_but_im_lazzy} to see the meaning and

 correct the "w01s3" word and i found out the correct one is 'worse' => "w0rs3"

 so i edited the flag and it worked and i got the chicken Challenge

FLAG: byuctf{th3r3_4r3_3ven_w0rs3_es0l4ngs_but_1m_lazzy}
