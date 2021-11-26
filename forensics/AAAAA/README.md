# AAAAA
AAAAA. That's all

download [AAAAA](AAAAA)

Okay - first of all, like always I run `file` on this AAAAA file.
This will tell us, that this is a data file. After that, I tried binwalk. BÄM
There is an image included. 
My colleague uses [CyberChef](https://gchq.github.io/CyberChef/) for this. There you can import the file and run *Extract files* on.
I just used `foremost`. This will create a folder `output` where you'll find another folder `png` in it.
Just go there and you will find the sweet little flag.

> TFCCTF{Gr4phic_d35ign_is_my_p455ion}
