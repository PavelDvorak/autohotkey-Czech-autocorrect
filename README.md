# Autocorrect for the Czech language (for autohotkey)
I use EN-US keyboard but have to often type in Czech. 

Here is a list of some 184k words containing special characters (such as ščřžýáěďťň).
For example, if you type the following sentence:
> Kdyz jsem ja slouzil to prvni leto, vyslouzil jsem si kuratko za to.

it will immediately get converted to:

> Kdy**ž** jsem j**á** slou**ž**il to prvn**í** l**é**to, vyslou**ž**il jsem si ku**řá**tko za to.

## Details and known issues
* The script is largely based on the complete list of Czech words, retrieved from 
[here](http://ucnk.korpus.cz/srovnani10.php).
* Only words longer than 3 letters **and** containing special characters are included.
* The script was created by brute force: in one column I kept the list with special characters,
in another column I removed the special characters. Hence there are many (over 9000) duplicates, such as:
````autohotkey
::aktualizovany::aktualizovaný
::aktualizovany::aktualizovány
````
or 
````autohotkey
::barevne::barevné
::barevne::barevně
````
The script is still a work in progress, but it serves me well. 
Let me know what you think!
