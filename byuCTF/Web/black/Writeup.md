### Black - Writeup
### ============


## Challenge

```black
One cool thing about Vue is that it's really hard to figure out what's going on in the page

Flag format - `byuctf{Phrase Separated By Spaces}`

`http://black.byuctf.xyz`
```


This Challenge made me a bit blind and hate vue js :D

lets go, first thing the website wasn't have anything interested

inputs/vulenrabilities and vue js obuscated the js code to make it

unreadable so i scrolled at the bottom and fired inspector and

started see how website change.

while i was moving my mouse away there

was a word has fade in "have fun!"

i understand how's website going in inspector there were some divs

with ids pt1, pt2 once i moused over on them they showed parties for

photos qr codes and be added in site source in inspector, so i

collected all qr codes they were 8 photos

![qr_parties](https://github.com/0x6DEF/byuCTF/blob/main/byuCTF/Web/black/partiesblack.png)

and i combined them as a one valid QR Code, 

![validQR](https://github.com/0x6DEF/byuCTF/blob/main/byuCTF/Web/black/qrcodesBlack/combined.png)

after i scanned it i got a url

"(http://black.byuctf.xyz/index_/)"

another page like previous one i used inspector to see the elements

there was a video i changed the width and height to see it, its a

rickroll video :( but i noticed there were some words shown in the

video not shown in the real video on youtube i wrote them : And Our

Home Oh Native Land Canada*** looks like be a canada anthem maybe i

just slaped it on google and first result was wiki article, and yeah

it a canada anthem

![anthem](https://github.com/0x6DEF/byuCTF/blob/main/byuCTF/Web/black/Pasted%20image%2020220529173208.png)

i compared the original anthem with my ones and i

re-arranged them to be a flag and i got Black Challenge Finally

FLAG: byuctf{Oh Canada Our Home And Native Land}
