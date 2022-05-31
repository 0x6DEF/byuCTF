# The Villain Writeup
#### =======================

### Challenge
```The-Villain

I've been hacked! Someone took a precious photo of mine and secured it in a password-protected ZIP folder. They taunted me by saying that the password is based on their personal life, but I'll never figure out who it is. I beg to differ! But all I've been able to find so far is this photo of my friend communicating with them, can you help me?
```

Challenge provides 2 files, one Screenshot.png and encrypted.zip


i download both and started with the img first i extracted the image metadata

and i found an google drive url [GooleDrive](https://docs.google.com/document/d/1BnPoqSl7GQOST__5iR7Xv7lYB8kSIxFsLYSq9PXaJFY/edit)

![villainempty.png](https://github.com/0x6DEF/byuCTF/blob/main/byuCTF/Forensics/thevillain/villainempty.png)

nothing interesting for the first time and the zip file requires a password

i fired pw cracker while it was running i returned to drive again

and i started to copy the content once i highlighted the content for copying

i saw there is a small sentence: Message for Astoria Villin

![astoria.png](https://github.com/0x6DEF/byuCTF/blob/main/byuCTF/Forensics/thevillain/astoria.png)

of course i started to search with this name in twitter/facebook

and i found a fb account and twitter with this username [Facebook](https://www.facebook.com/astoria.villin) | [Twitter](https://twitter.com/AstoriaVillin)

![astoriafb](https://github.com/0x6DEF/byuCTF/blob/main/byuCTF/Forensics/thevillain/astoriafb-.png)

discovering the account i stared to collect everything that can be used for password

and the challenge says: They taunted me by saying that the password is based on their personal life

so the password related to her life

i collected her husband name: Jonathan

and her pet name: Hoppy Boi

husband not worked


so i tried pet name without spaces: HoppyBoi

and it worked, and got the flag

FLAG: byuctf{b3t_Y0U_c4nt_f1nd_D33ZNU7S!}

#### Screenshots:

![flag](https://github.com/0x6DEF/byuCTF/blob/main/byuCTF/Forensics/thevillain/flag.png)
