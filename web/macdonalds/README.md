# MACDONALDS
I'm a huge Ronald fan. My fan page doubles down as my cloud storage page! You'll never find my secrets!

[http://server.challenge.ctf.thefewchosen.com:1339](http://server.challenge.ctf.thefewchosen.com:1339)

# Todos

Okay, given the hint for the webserver he is hosting on his macos we were looking into some google research.
There are quite some issues with this `.DS_Store` files.

Okay lets try, if we can get one of those! And found it [server.challenge.ctf.thefewchosen.com:1339/.DS_Store](server.challenge.ctf.thefewchosen.com:1339/.DS_Store).
Then lets cat the shit out of that.

What we can see, is that the the files from the webservice are listet... beside some other not readable infos.

We can see the
 - index.php
 - style.css
 - style.scss

and... 

 - secrets ...?

Okay lets try to get this `DS_Store` file in the `secret` folder.

[server.challenge.ctf.thefewchosen.com:1339/secrets/.DS_Store](server.challenge.ctf.thefewchosen.com:1339/secrets/.DS_Store). Oha - that works... I saved the file as `secret_DS_Store`. In this file we can see another `php` file: `5973b4cc1d61c110188ee413cddb8652.php`.

Lets have a further look into that! [server.challenge.ctf.thefewchosen.com:1339/secrets/5973b4cc1d61c110188ee413cddb8652.php](server.challenge.ctf.thefewchosen.com:1339/secrets/5973b4cc1d61c110188ee413cddb8652.php). 

Oh boy, there it is... the flag:

> TFCCTF{.D5_S70r3_1s_s0_4nn0ying_wh3n_c0mp1l1ng_j4rs_y0urs3lf}
