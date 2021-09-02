---
title: Gravithon CTF 2021
author: Vishnu Sudhakaran
date: 2021-09-02 11:30:00 +0800
categories: [CTF-WriteUps]
tags: [ ctf ]
---

![](/assets/img/posts/gravithon21/7th.png)

I secured 7th position in the 24 hour **Gravithon CTF 2021** at the Indian Tech Fest.

# Challenges-Writeups

# Welcome 

## Warm Welcome

![](/assets/img/posts/gravithon21/warm-wel/1.png)

Flag is given there.

```
gravithon{W3lc0me&Welcome_t0_Gr4v1th0n_2021}
```
___

## You Got it

![](/assets/img/posts/gravithon21/you-got-it/1.png)

You can find Hashtag on their Linkedin page.

![](/assets/img/posts/gravithon21/you-got-it/2.png)

```
gravithon{#feelthegravity}
```
___

## How About Some Exploring the Things

![](/assets/img/posts/gravithon21/how-about/1.png)

You can find flag on general chat in that discord server.

![](/assets/img/posts/gravithon21/how-about/2.png)

```
gravithon{Xpl0re_Th3Uns33n@_Cyb3rXpl0re}
```
___

## ReadMe.md

![](/assets/img/posts/gravithon21/ReadMe/1.png)

You can find flag on challenge description.

```
gravithon{LifeSaverGravithon}
```
___

# Easy

## Letters

![](/assets/img/posts/gravithon21/letters/1.png)

Challenge:
```
xirmzkyfe{jyzwk_zj_fwtflitv_vrjp}
```

It's `ROT9` cipher, We already know the flag format, when rotating the letters each letters rotates 9 times to get our flag format. that is **g** will assigned as **x**, [Decode](https://gchq.github.io/CyberChef/#recipe=ROT13(true,true,false,9)&input=eGlybXpreWZle2p5endrX3pqX2Z3dGZsaXR2X3ZyanB9) it and get the flag.

![](/assets/img/posts/gravithon21/letters/2.png)

```
gravithon{shift_is_ofcource_easy}
```
___

## Robbery

![](/assets/img/posts/gravithon21/robbery/1.png)

Challenge:
```
miaqqmoca{P4n3_j0I_pw3j_Srpb3Y0yq3??}
```

It's `Vigenère cipher`, but key is missing, i guessed `gravithon` as key, it give right flag format, So need to find rest of the key.
With the help of `ReadMe.md` challenge, you will get the key that is `gravithonislove`.

![](/assets/img/posts/gravithon21/robbery/2.png)

```
gravithon{H4v3_y0U_us3d_Brut3F0rc3??}
```
___

## TIK TOK

![](/assets/img/posts/gravithon21/tik-tok/1.png)

Challenge:
```
-- ----- .-. ... ...-- .. ... ....- .-.. .-- .- -.-- ... -... ...-- . ... -
```

It's a `Morse Code`. [Decode](https://www.dcode.fr/morse-code) to get your flag.

![](/assets/img/posts/gravithon21/tik-tok/2.png)

```
gravithon{M0RS3IS4LWAYSB3EST}
```
___

## Binary always Awsome

![](/assets/img/posts/gravithon21/binary-always/1.png)

Challenge:
```
000000000000000000000000000000110010000010000000000010000000000000000000000010000000000000000000000000000000011011011011001111010010010000000000000000000000000000000000000000000100010000000000000100011011000000000000000000000000000000000000000000000000000000000000000100010010000000000000000000000000000000000100011011100010000000000000000000000000000000000100001001001001001001001001001001001001001001001100010001100011011001001001100010010001001001001001001001001001001001100000000000000000000000000000000000100011011000000000000100010010001001001001001100100011011001001001100010010000100001001001001001001001100001001001001001001001001100011000000000100010000000000000000000000000000000000000000000000000000000000000000000100011000000000000000000000000000000000000000000000000100000000000000000000000000100010001001100
```

It's a `Binary Fuck Language`. [Decode](https://www.dcode.fr/binaryfuck-language) to get your flag.

![](/assets/img/posts/gravithon21/binary-always/2.png)

```
gravithon{Th3s3_Pr0gr4mm1ng_Sucks}
```
___

## Everything is Not Visible

![](/assets/img/posts/gravithon21/every-thing/1.png)

Here the given link was [https://bit.ly/3mr9p5C](https://bit.ly/3mr9p5C) , With help of Browser's `Network Monitor` Tab, you can see the all contents that loading, and it is double shorted URL, that is `bit.ly` and `tinyurl` from the name of that url we get our flag.

![](/assets/img/posts/gravithon21/every-thing/2.png)

```
gravithon{Y0u4r3S4f3}
```
___

## So Loudd

![](/assets/img/posts/gravithon21/so-loud/1.png)

Challenge: [morse.wav](https://github.com/an0n4ce/blog/raw/main/assets/img/posts/gravithon21/so-loud/morse.wav)

It's a `Morse Code` audio, We can use [Morse Decoder](https://morsecode.world/international/decoder/audio-decoder-adaptive.html) to get the flag, Upload and play the audio.
The decrypted message will be our flag.

![](/assets/img/posts/gravithon21/so-loud/2.png)

```
gravithon{1S TH1S A M0RS3 C0D3?}
```
___

## Fly High to Tianjin

![](/assets/img/posts/gravithon21/fly-high/1.png)

Challenge:
```
395f4dfc82f56b796b23c3fa1b5150cbe568d71e
```

It's a `SHA1` hashing algorithm. I used [CrackStation](https://crackstation.net/) to crack the hash.

![](/assets/img/posts/gravithon21/fly-high/2.png)

```
gravithon{Unimaginatively}
```
___

# Medium

## Clone And Clone

![](/assets/img/posts/gravithon21/clone/1.png)

Challenge:
```
3P7T:R4@?Yj_U5p8_S%5#_R`tA
```
It looks like a `ROT47` string, When we do `ROT13` and `ROT47` we, get our flag like this ` brfvitcon{H0wd4g0uTdR0t18} `.

![](/assets/img/posts/gravithon21/clone/2.png)

The flag has 3 words, first and last is set for us. what i done here guessed the middle word. that is `H0w_4b0uT_R0t18`

```
gravithon{H0w_4b0uT_R0t18}
```
___

## Not that Tough

![](/assets/img/posts/gravithon21/note-that/1.png)

Challenge:
```
MFEFEMDDJBGTMTDZHEYGCVZVGVSFQSTTJRWU45TCKM4WWYRSGVWGIMTMGBQUOZDZLFMFU4DEI5UHMYTNGV3GKVZZGFMVQSTMMJWTSMA
```
It's multiple encoded string, that is first `Base32` then `Base64`, gives a shorted url [https://tinyurl.com/donewithgravithonnoyouarenot](https://tinyurl.com/donewithgravithonnoyouarenot)

![](/assets/img/posts/gravithon21/note-that/2.png)

the link going for another encoded cipher that is `Pikalang`, 

```
pi pi pi pi pi pi pi pi pi pi pika pipi pi pipi pi pi pi pipi pi pi pi pi pi pi pi pipi pi pi pi pi pi pi pi pi pi pi pichu pichu pichu pichu ka chu pipi pipi pipi ka ka ka ka ka pikachu pipi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pikachu pichu ka ka ka ka ka ka ka ka ka ka ka ka ka ka pikachu pipi ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka pikachu pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pikachu pichu ka ka ka pikachu pipi ka ka ka ka pikachu ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka pikachu pi pi pi pi pi pi pi pikachu pichu pi pi pi pi pikachu pipi pi pi pi pi pi pi pi pi pikachu ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka pikachu pichu ka ka ka ka pikachu pipi pi pi pi pi pi pi pi pikachu ka ka ka ka ka ka ka pikachu pichu pi pi pi pi pikachu pipi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pikachu pichu ka ka ka pikachu pipi ka pikachu pichu pi pi pikachu pipi ka ka ka ka ka ka ka ka ka ka ka ka ka ka pikachu pichu ka ka ka pikachu pipi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pikachu ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka pikachu ka ka ka ka ka ka ka ka ka ka ka ka ka ka ka pikachu pichu pi pikachu pipi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pi pikachu pichu pi pi pi pikachu pipi ka ka ka ka ka ka ka ka pikachu pi pi pi pi pi pikachu pi pi pi pi pi pi pi pi pi pi pi pi pi pikachu 
```
[Decode](https://www.dcode.fr/pikalang-language) to get our flag.

![](/assets/img/posts/gravithon21/note-that/3.png)

```
gravithon{Ar3_y0u_f4n_0f_4n1m3_0r_P1k4chu}
```
___

## Map

![](/assets/img/posts/gravithon21/map/1.png)

Challenge:
```
22434223_4223_42212322_55_234234313551_34553131423344
```
I just searched given string on `google` and found 3 results.

![](/assets/img/posts/gravithon21/map/2.png)

There is Japanese CTF writeups, from that we get our [flag](https://yocchin.hatenablog.com/category/writeup?page=1608559860).

![](/assets/img/posts/gravithon21/map/3.png)

```
gravithon{THIS_IS_JUST_A_SIMPLE_MAPPING}
```
___

## 64 and 64

![](/assets/img/posts/gravithon21/64-64/1.png)

Challenge: [64Base64.txt](https://github.com/an0n4ce/blog/raw/main/assets/img/posts/gravithon21/64-64/64Base64.txt)

it's a 38 times `base64` encoded string, Decode to get your flag.

```
gravithon{l00ks_l1ke_4_l0t_0f_64s}
```
___

## Rainbow Of Colors

![](/assets/img/posts/gravithon21/rainbow/1.png)

Challenge: [Rainbow_of_Colors.JPG](https://github.com/an0n4ce/blog/raw/main/assets/img/posts/gravithon21/rainbow/Rainbow_of_Colors.JPG)

![](/assets/img/posts/gravithon21/rainbow/2.png)

The challenge is about `Hexahue Cipher`. [Decode](https://www.dcode.fr/hexahue-cipher) and get your flag.

```
gravithon{should,fl5g4,b3,st1cky,or,n0t}
```
___

# Hard

## I lost my Way

![](/assets/img/posts/gravithon21/i-lost-my/1.png)

Challenge: [Who_am_I_.txt](https://github.com/an0n4ce/CTF-Write-Ups/blob/master/Gravithon-CTF-21/I-lost-my-Way/img/Who_am_I_.txt)

It's multiple encoded text file that is `base32` and `base64`. 

![](/assets/img/posts/gravithon21/i-lost-my/2.png)

After that we will get `PNG` image file [download](https://github.com/an0n4ce/blog/raw/main/assets/img/posts/gravithon21/i-lost-my/download.png) it and open to get your flag. Wrap it in all Capital letters as per the instruction.

```
gravithon{F1N4LLY_Y0U_CR34T3D_B34UT1FUL_IM4G3}
```
___

# Forensic

## Look into it

![](/assets/img/posts/gravithon21/look-into/1.png)

Challenge: [secret.jpeg](https://github.com/an0n4ce/blog/raw/main/assets/img/posts/gravithon21/look-into/secret.jpeg)

Use `exiftool` to get your flag.
```
exiftool secret.jpeg
```
![](/assets/img/posts/gravithon21/look-into/2.png)

```
gravithon{Y0u_4r3_G00d_4t_M3t4D4t4}
```
___

## I can See You

![](/assets/img/posts/gravithon21/i-can-see/1.png)

Challenge: [snow.zip](https://github.com/an0n4ce/blog/raw/main/assets/img/posts/gravithon21/i-can-see/snow.zip)

From the given file name `snow.zip` we know it's a `snow tool` challenge. Here i used [stegsnow](http://manpages.ubuntu.com/manpages/bionic/man1/stegsnow.1.html) to get the flag.

stegsnow is a program for concealing messages in text files by appending tabs  and  spaces on  the  end  of lines, and for extracting messages from files containing hidden messages. Tabs and spaces are invisible to most text viewers, hence  the  steganographic  nature  of this encoding scheme.

![](/assets/img/posts/gravithon21/i-can-see/2.png)

After extarcting the file we get 3 more files, There is a fake flag, and our challange, and passwd that is in `.secret.txt`

![](/assets/img/posts/gravithon21/i-can-see/3.png)

Use `stegsnow` to get the flag and give passwd as `welc0me_to_gravithon2021_ctf` from `.secret.txt`

```
stegsnow -C -Q -p welc0me_to_gravithon2021_ctf snow/challenge.txt

```

![](/assets/img/posts/gravithon21/i-can-see/4.png)

```
gravithon{i5_it_c0ld_ov3r_th3re}
```

### Thank you for reading my writeup!!


