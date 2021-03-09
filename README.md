# UMCTF Competition Noob's Hackathon 公開組


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

