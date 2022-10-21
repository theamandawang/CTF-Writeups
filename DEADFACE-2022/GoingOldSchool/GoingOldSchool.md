Looking at the braille at the bottom of ```Old_School_sm.png```, it reads as
```port #47980```

So, I connected to port #47980 of env.deadface.io via the command:

```nc env.deadface.io -p 47980```

After scanning the port, we get the result ```GOBLINS```.

Looking at the image itself, we notice that we have a matrix with a reversed alphabet on the top and leftmost sides.

This is an obvious marker for a Vigenère cipher; it looks like the alphabet is the reversed alphabet from the image, and the key is ```GOBLINS```.

We put ```DT UFAWDL IQYXFKVL``` into the Vigenère cipher solver on ```dcode.fr``` to solve!


We get ```flag{WE STRIKE TOMORROW}```
