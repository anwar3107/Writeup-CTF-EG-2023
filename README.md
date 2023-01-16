---------------------------------------------------------------------------
# Writeup-CTF-EG-2023
---------------------------------------------------------------------------

## Thirsty
![Thirsty Question](https://github.com/anwar3107/Writeup-CTF-EG-2023/blob/main/thirsty/ques.png)
| Files         |
| ------------- |
| [menu.zip](https://github.com/anwar3107/Writeup-CTF-EG-2023/blob/main/thirsty/Menu.zip)      |
| [place.zip](https://github.com/anwar3107/Writeup-CTF-EG-2023/blob/main/thirsty/Place.zip)      |
| [pokemon.jpg](https://github.com/anwar3107/Writeup-CTF-EG-2023/blob/main/thirsty/pokemon.png)      |

---------------------------------------------------------------------------

So the first unlocked file we got is Pokemon.jpg and when we open it up we got the maps where did Ash go for drinks

![pokemon.jpg](https://github.com/anwar3107/Writeup-CTF-EG-2023/blob/main/thirsty/pokemon.jpg)      

After doing some OSINT we got the location is “Starbucks Medan Gopeng” and put the name in Place.zip as the password

![gmap.jpg](https://github.com/anwar3107/Writeup-CTF-EG-2023/blob/main/thirsty/gmap.png)

![place.jpg](https://github.com/anwar3107/Writeup-CTF-EG-2023/blob/main/thirsty/place.png)  

We get the next clue! So the picture showed that the owner of the account liked eliteghostmy post on instagram so we gonna do some OSINT on the eliteghost page to get the owner of the account

![photo_2023-01-11_19-08-09.jpg](https://github.com/anwar3107/Writeup-CTF-EG-2023/blob/main/thirsty/photo_2023-01-11_19-08-09.jpg)

Seeing the post likes we’ve seen identical picture of IG account named nnshuada._ and it got 1 post about starbucks menu 😋

![like.jpg](https://github.com/anwar3107/Writeup-CTF-EG-2023/blob/main/thirsty/like.png)
![menu-acc.jpg](https://github.com/anwar3107/Writeup-CTF-EG-2023/blob/main/thirsty/menu-acc.png)

So just like the zip name (Menu.zip) we need to put the menu as password : MOCHAPRALINEFRAPPUCCINO

![menu.jpg](https://github.com/anwar3107/Writeup-CTF-EG-2023/blob/main/thirsty/menu.png)

Both of files share the same password and what we get is mp4 file and txt file that shown lyrics of the song
![pokemon.jpg](https://github.com/anwar3107/Writeup-CTF-EG-2023/blob/main/thirsty/pokemon.png)
![lyrics.jpg](https://github.com/anwar3107/Writeup-CTF-EG-2023/blob/main/thirsty/lyrics.png)

as we analyzed the cipher on the video it’s actually using Book Cipher method but book cipher using page:line:word so we need to minimize the cipher to line:word:alphabets

```

eg. 12:5:2
12th line:5th word:2nd alphabet

```
And voila we got E as our first alphabet of the flag ⛳
As we keep decipher the full flag will be
```
EG{REST_WITH_COFFEE}
```

