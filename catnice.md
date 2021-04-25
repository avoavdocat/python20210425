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
numbers : 51099 8679 82518 98813 63684 89100 ...  94575

answer : 99754

Ans: CTF{yoUaReInth33RdpL4c3}


## 1~100

cat.py-
```python
from pwn import *

ip="120.114.62.214"

port=2403

r = remote(ip, port)


for i in range(1,101):

	r.recvuntil("wave")
	
	r.recvuntil("?")
	
	r.sendline(str(i))
	
r.interactive()

```
---Ans: CTF{gOOD4tMatHYOUarE}



