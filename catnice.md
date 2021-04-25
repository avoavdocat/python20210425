# 4/25
## Base64 -
 import base64
 base64.b32base64.b64encode(b"BreakallCTF{happyhackinghighhaaha}")
Ans: b'QnJlYWthbGxDVEZ7aGFwcHloYWNraW5naGlnaGhhYWhhfQ==

 
## Base64 -
  base64.b32decode(b"IJZGKYLLIFGEYQ2UIZ5TS6BUHA2VMUZXO5UWS5CCLJMFKVLIJVSX2===")
Ans: b'BreakALLCTF{9x485VS7wiitBZXUUhMe}'


## Ascii -
BreakALLCTF{Amv0uDyervPtmVr9SSSK}
hello world -
[XD] % nc 120.114.62.214 2405
### ===== Welcome to CTF =====
You successfully reach this problem
Congratulation!!!
Wait for a few second, let me get you the flag

---Ans: Here you go : CTF{Hel10WorLD123}


## 3rd -
[XD] % nc 120.114.62.214 2400
===== Welcome to 3rd Game =====
Can you help me find the 3rd largest number?
All numbers are unique
----- Example -----
numbers : 1 9 7 3 6 2
answer : 6
----- Now You Turn -----
numbers : 51099 8679 82518 98813 63684 89100 32404 53862 75741 20314 42336 775 66544 76270 84853 72535 4359 55561 73522 21530 474 50132 39554 99975 17479 154 50483 54970 45538 38379 10719 86925 58167 12343 84032 63691 85881 63942 9192 20805 60381 87245 68171 99754 16637 92650 38501 38693 79384 87023 74457 85258 9579 27055 74882 44299 65397 82238 34557 47706 90678 77095 83582 25350 78482 96743 65774 37205 29011 64028 88297 63327 7366 60452 88691 1118 20677 15662 1747 13467 34912 14497 31838 45385 41372 68464 35047 85567 97010 24597 88299 82159 89949 98842 84952 99995 12752 96458 46749 94575
answer : 99754
Ans: CTF{yoUaReInth33RdpL4c3}

## 1~100

15:52 user@user-VirtualBox(10.0.2.15)[~] 
[XD] % gedit cat.py  
15:52 user@user-VirtualBox(10.0.2.15)[~] 
[XD] % python3 cat.py
cat.py-
from pwn import *
ip="120.114.62.214"
port=2403

r = remote(ip, port)
for i in range(1,101):
	r.recvuntil("wave")
	r.recvuntil("?")
	r.sendline(str(i))
r.interactive()

---Ans: CTF{gOOD4tMatHYOUarE}



