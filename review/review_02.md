# 2단원 복습 문제

## 1번
### a)
가까운 시간 안에 사용할 데이터를 저장한다.

### b)
범용 레지스터 : CPU에서의 연산에 사용될 데이터 또는 결과값을 저장한다.  
주기억장치 : 가까운 시간 안에 사용할 데이터를 저장한다.  

## 2번
### a)
0010 0011 0000 0100

### b)
1101

### c)
0010 1100 0101

## 3번
98 99 9A 9B 9C 9D 9E 9F A0 A1 A2

11개

## 4번
CD

## 5번
1회  
2211 카운터02   
2번 레지스터에 11 저장

2회   
3202 카운터04   
02번 셀에 2번 레지스터의 내용(11) 저장 

3회   
C000 카운터06   
종료

## 6번
x + y + z
1. x를 담고 있는 셀에서 1번 레지스터로 값 LOAD
2. y를 담고 있는 셀에서 2번 레지스터로 값 LOAD
3. 1번 레지스터와 2번 레지스터의 합을 3번 레지스터에 저장
4. z를 담고 있는 셀에서 4번 레지스터로 값 LOAD
5. 3번 레지스터와 4번 레지스터의 합을 5번 레지스터에 저장
6. 5번 레지스터의 값을 메모리에 저장

(2x) + y
1. x를 담고 있는 셀에서 1번 레지스터로 값 LOAD
2. 1번 레지스터와 1번 레지스터의 합을 2번 레지스터에 저장
3. y를 담고 있는 셀에서 3번 레지스터로 값 LOAD
4. 2번 레지스터와 3번 레지스터의 합을 4번 레지스터에 저장
5. 4번 레지스터의 값을 메모리에 저장

## 7번
### a)
7123

2번 레지스터와 3번 레지스터의 내용을 OR하여 그 결과를 1번 레지스터에 저장

### b)
40E1

E번 레지스터의 내용을 1번 레지스터에 MOVE

### c)
A304

3번 레지스터의 내용을 오른쪽으로 4번 ROTATE

### d)
B100

1번 레지스터와 0번 레지스터의 내용이 같으면 주소가 00인 셀에 위치한 명령으로 JUMP

### e)
2BCD

B번 레지스터에 CD(1100 1101)를 LOAD

## 8번
4비트 명령 코드 필드 = 최대 16개  
6비트 명령 코드 필드 = 최대 64개

## 9번
### a)
2677

### b)
1777

### c)
BA24

### d)
A403

### e)
81E2

## 10번
156C    
166D   
6056 (부동소수점 표현으로 ADD)   
306E   
C000

## 11번
### a)
변경한다.

### b)
무관하다.

### c)
읽어온다.

### d)
변경한다.

### e)
무관하다.

## 12번
### a)
2655

6번 레지스터에 16진수 55를 LOAD하라.

### b)
0x55 = 0101 0101

## 13번
### a)
1221

### b)
2134

## 14번
### a)
1202 : 02번 셀의 내용을 2번 레지스터에 LOAD   
3242 : 2번 레지스터의 내용을 42번 셀에 STORE   
C000 : 종료

### b)
0x32 = 0011 0010

### c)
06

## 15번
1C03 : 03번 셀의 내용(03)을 C번 레지스터에 LOAD    
2B03 : 0x03을 B번 레지스터에 LOAD   
5ABC : B번 레지스터와 C번 레지스터의 내용을 2의 보수 표현으로 ADD하여 A번 레지스터에 저장     
3A00 : A번 레지스터의 내용을 00번 셀에 STORE     
C000 : 종료

### a)
06

### b)
0A

## 16번
### a)
00, 02, 04

### b)
06

## 17번 
2004 : 0번 레지스터에 0x04 저장   
2101 : 1번 레지스터에 0x01 저장   
4012 : 1번 레지스터의 내용을 2번 레지스터에 MOVE   
5112 : 1번 레지스터의 내용과 2번 레지스터의 내용을 2의 보수 ADD하여 1번 레지스터에 저장   
B10C : 1번 레지스터와 0번 레지스터의 내용이 같으면 0C번 셀(C000)로 JUMP   
B006 : 0번 레지스터와 0번 레지스터의 내용이 같으면 06번 셀(5112)로 JUMP   
C000 : 종료

### a)
0x04

### b)
0x04

### c)
0E

## 18번
2000 : 0번 레지스터에 0x00 저장   
2202 : 2번 레지스터에 0x02 저장   
2304 : 3번 레지스터에 0x04 저장    
B3FC : 3번 레지스터와 0번 레지스터의 내용이 같으면 FC번 셀(C000)로 JUMP    
5002 : 0번 레지스터의 내용과 2번 레지스터의 내용을 2의 보수 ADD하여 0번 레지스터에 저장     
B0F6 : 0번 레지스터와 0번 레지스터가 같으면 F6번 셀(B3FC)로 JUMP    
C000 : 종료

0x04

## 19번
100만분의 11초

## 20번
※ 실행 순서대로 정리    
1220 : 20번 셀의 내용(12)을 2번 레지스터에 저장    
3230 : 2번 레지스터의 내용을 30번 셀에 저장    
B021 : 0번 레지스터와 0번 레지스터의 내용이 같으면 21번 셀(2032)로 JUMP     
2032 : 0번 레지스터에 0x32 저장     
30B0 : 0번 레지스터의 내용을 B0번 셀에 저장    
2124 : 1번 레지스터에 0x24 저장    
C000 : 종료

### a)
0번 레지스터 : 0x32    
1번 레지스터 : 0x24    
2번 레지스터 : 0x12    

### b)
0x12

### c)
0x32

## 21번 
※ 실행 순서대로 정리    
B0B0 : 0번 레지스터와 0번 레지스터의 내용이 같다면 B0번 셀(B0AF)로 JUMP    
B0AF : 0번 레지스터와 0번 레지스터의 내용이 같다면 AF번 셀(B0B0)로 JUMP    

컴퓨터가 종료되지 않고 무한 반복된다.

## 22번
※ 실행 순서대로 정리     
25B0 : 5번 레지스터에 0xB0 저장    
3504 : 5번 레지스터의 내용을 04번 셀(C0→B0)에 저장     
B000 : 0번 레지스터와 0번 레지스터의 내용이 같다면 00번 셀(25B0)로 JUMP

영원히 멈추지 않는다.

## 23번
### a)
11D8   
31B3

### b)
11D8    
12B3    
31B3    
32D8

### c)
00-01 1144 : 44번 셀의 내용을 1번 레지스터에 저장     
02-03 2000 : 0번 레지스터에 00 저장     
04-05 B10C : 0번 레지스터의 내용이 1번 레지스터의 내용과 같으면 0C로 JUMP   
06-07 22FF : 2번 레지스터에 FF 저장    
08-09 3246 : 2번 레지스터의 내용을 46번 셀에 저장     
0A-0B B010 : 0번 레지스터와 0번 레지스터의 내용이 같으면 10번 셀로 JUMP     
0C-0D 2301 : 3번 레지스터에 01 저장    
0E-0F 3346 : 3번 레지스터의 내용을 46번 셀에 저장    
10-11 C000 : 종료

## 24번
> 코어워즈(Core Wars)라는 게임은 한 컴퓨터의 메모리상의 서로 다른 위치에 저장되어 서로 싸우는 두 프로그램 사이에서 진행된다.
> 컴퓨터는 한 프로그램의 명령 하나를 실행한 다음에는 다른 프로그램의 명령 하나를 실행하는 방식으로 두 프로그램 사이를 오간다.
> 각 프로그램의 목표는 상대 프로그램이 들어있는 메모리에 엉뚱한 데이터를 써넣음으로써 상대 프로그램에 오동작을 일으키는 것인데,
> 서로 상대방의 위치를 모른다.

### a)
> Vole 기계어를 사용하여 코어워즈와 비슷한 프로그램을 작성하되, 크기를 최소화함으로써 자신을 방어하는 전략을 반영하라.

### b)
> Vole 기계어를 사용하여 코어워즈와 비슷한 프로그램을 작성하되, 자신의 위치를 옮김으로써 상대 프로그램으로부터의 공격을 피하는 전략을 반영하라.
> 조금 더 구체적으로 표현하자면, 주소 00에서 시작하는 프로그램을 작성하되, 이 프로그램은 자신을 주소 70으로 복사한 다음 주소 70으로 점프한다.

### c)
> 계속 새로운 주소로 자신의 위치를 변경하도록 (b)의 프로그램을 확장하라.
> 새로운 위치는 이전 위치에 70을 더하여 계산하라. 즉, 처음 위치는 00, 두 번째 위치는 70, 세 번째 위치는 E0, 그 다음 위치는 50 등과 같이 계산된다.

## 25번
11A1 : A1번 셀의 내용을 1번 레지스터에 저장   
12A2 : A2번 셀의 내용을 2번 레지스터에 저장   
13A3 : A3번 셀의 내용을 3번 레지스터에 저장   
6412 : 1번 레지스터와 2번 레지스터의 내용을 부동 소수점 ADD하여 4번 레지스터에 저장   
6534 : 3번 레지스터와 4번 레지스터의 내용을 부동 소수점 ADD하여 5번 레지스터에 저장   
35A4 : 5번 레지스터의 내용을 A4번 셀에 저장   
C000 : 종료

## 26번
※ 실행 순서대로 정리   
20C0 : 0번 레지스터에 C0 저장   
3004 : 0번 레지스터의 내용을 04번 셀(00→C0)에 저장   
C000 : 종료

04번 셀에 대한 자가 수정이 일어나 정상 종료된다.

## 27번
08번 셀로 계속하여 JUMP가 일어나 컴퓨터가 종료되지 않고 무한 반복된다.

## 28번
30 20   
31 03   
32 21   
33 01   
34 22   
35 00   
36 23   
37 10   
38 14   
39 00   
3A 34   
3B 10   
3C 52   
3D 21   
3E 53   
3F 31   
40 32    
41 39   
42 33   
43 3B    
44 B2    
45 48    
46 B0    
47 38    
48 C0   
49 00   

2003 : 0번 레지스터에 03 저장   
2101 : 1번 레지스터에 01 저장   
2200 : 2번 레지스터에 00 저장  
2310 : 3번 레지스터에 10 저장   
1400 : 00번 셀의 내용을 4번 레지스터에 저장   
3410 : 4번 레지스터의 내용을 10번 셀에 저장   
5221 : 2번 레지스터와 1번 레지스터의 내용을 2의 보수 ADD하여 2번 레지스터에 저장   
5331 : 3번 레지스터와 1번 레지스터의 내용을 2의 보수 ADD하여 3번 레지스터에 저장   
3239 : 2번 레지스터의 내용을 39번 셀에 저장   
333B : 3번 레지스터의 내용을 3B번 셀에 저장   
B248 : 2번 레지스터와 0번 레지스터의 내용이 같다면 48번 셀로 JUMP    
B038 : 0번 레지스터와 0번 레지스터의 내용이 같다면 38번 셀로 JUMP   
C000 : 종료

※ 실행 순서대로 정리   
2003 : 0번 레지스터 03   
2101 : 1번 레지스터 01   
2200 : 2번 레지스터 00   
2310 : 3번 레지스터 10   
1400 : 00번 셀의 내용을 4번 레지스터에 저장   
3410 : 4번 레지스터의 내용을 10번 셀에 저장   
5221 : 2번 레지스터 01   
5331 : 3번 레지스터 11   
3239 : 39번 셀(00→01)   
333B : 3B번 셀(10→11)   
B248 : 정상 실행   
B038 : 38번 셀(1401)로 JUMP   

1401 : 01번 셀의 내용을 4번 레지스터에 저장   
3411 : 4번 레지스터의 내용을 11번 셀에 저장   
5221 : 2번 레지스터 02   
5331 : 3번 레지스터 12   
3239 : 39번 셀(01→02)   
333B : 3B번 셀(11→12)   
B248 : 정상 실행   
B038 : 38번 셀(1402)로 JUMP   

1402 : 02번 셀의 내용을 4번 레지스터에 저장   
3412 : 4번 레지스터의 내용을 12번 셀에 저장   
5221 : 2번 레지스터 03   
5331 : 3번 레지스터 13     
3239 : 39번 셀(02→03)   
333B : 3B번 셀(12→13)   
B248 : 48번 셀(C000)로 JUMP   
C000 : 종료

2번 레지스터의 내용이 0번 레지스터의 내용과 같아질 때까지 반복적으로 실행된다.

## 29번
BRXY
1. R번 레지스터의 내용과 0번 레지스터의 내용을 비교한다.
2. 두 레지스터의 내용이 같다면 XY를 프로그램 카운터에 넣는다.
3. 같지 않다면 아무 일도 수행하지 않는다. (프로그램이 정상 실행된다.)

## 30번
5RST
1. S번 레지스터의 내용과 T번 레지스터의 내용을 2의 보수 표현으로 더한다.
2. 그 합을 R번 레지스터에 넣는다.

## 31번
6RST
1. S번 레지스터의 내용과 T번 레지스터의 내용을 부동소수점 표현으로 더한다.
2. 그 합을 R번 레지스터에 넣는다.

## 32번
4번 레지스터 : 3A   
5번 레지스터 : C8

### a)
5045 : 4번 레지스터와 5번 레지스터의 내용을 2의 보수 표현으로 ADD하여 0번 레지스터에 저장한다.

0번 레지스터 : 0000 0010 = 02

### b)
6045 : 4번 레지스터와 5번 레지스터의 내용을 부동소수점 표현으로 ADD하여 0번 레지스터에 저장한다.

0번 레지스터 : 1 010 1100 = AC

### c)
7045 : 4번 레지스터와 5번 레지스터의 내용을 OR하여 0번 레지스터에 저장한다.

0번 레지스터 : 1111 1010 = FA

### d) 
8045 : 4번 레지스터와 5번 레지스터의 내용을 AND하여 0번 레지스터에 저장한다.

0번 레지스터 : 0000 1000 = 08

### e)
9045 : 4번 레지스터와 5번 레지스터의 내용을 XOR하여 0번 레지스터에 저장한다.

0번 레지스터 : 1111 0010 = F2

## 33번
### a)
1144  
31AA

### b)
AND 1111 0000 = F0

1134    
22F0   
8312    
3334

### c)
AND 1111 0000 = F0    
AND 0000 1111 = 0F

11A6   
22F0   
8312 : 상위 4비트만 살리기    
14A5   
250F    
8645 : 하위 4비트만 살리기    
7736 : OR로 합치기    
37A6

### d)
AND 0000 1111 = 0F

11A5   
220F    
8312 : 하위 4비트만 살리기 (0000 XXXX)    
4034 : 복사본 만들기 (0000 XXXX)   
A304 : 하위 4비트를 상위 4비트로 옮기기 (XXXX 0000)   
7534 : OR로 합치기   
35A5

## 34번
### a)
101001

### b)
000000

### c)
000100

### d)
110001

### e)
111001

### f)
111110

### g)
010101

### h)
111111

### i)
010000

### j)
101101

### k)
000101

### l)
001010

## 35번
### a)
OR 1111 0000

### b)
XOR 1000 0000

### c)
XOR 1111 1111

### d)
AND 1111 1110

### e)
OR 0111 1111

### f)
AND 1111 1111 0000 0000 1111 1111

### g)
XOR 1111 1111 1111 1111 1111 1111

### h)
OR 1111 1111 1111 1111 1111 1111

## 36번
### a)
```python
pattern = 0b01001011
mask = 0b11110000
print(bin(pattern | mask))
```

### b)
```python
pattern = 0b01001011
mask = 0b10000000
print(bin(pattern ^ mask))
```

### c)
```python
pattern = 0b01001011
mask = 0b11111111
print(bin(pattern ^ mask))
```

### d)
```python
pattern = 0b01001011
mask = 0b11111110
print(bin(pattern & mask))
```

### e)
```python
pattern = 0b01001011
mask = 0b01111111
print(bin(pattern | mask))
```

### f)
```python
pattern = 0b111111111111111111111111
mask = 0b111111110000000011111111
print(bin(pattern & mask))
```

### g)
```python
pattern = 0b010101110101101001101100
mask = 0b111111111111111111111111
print(bin(pattern ^ mask))
```

### h)
```python
pattern = 0b010101110101101001101100
mask = 0b111111111111111111111111
print(bin(pattern | mask))
```

## 37번
> 8비트 입력 열에 적용될 경우 입력이 1000 0001일 경우에만 출력 비트 열 전체가 0이 되는 논리 연산과 마스크를 제시하라.

XOR 1000 0001

## 38번
```python
pattern = 0b10000001
mask = 0b10000001
print(bin(pattern ^ mask))
```

## 39번
> 8비트 입력 열에 적용될 경우 입력 비트 열의 시작 비트와 마지막 비트가 모두 1일 경우 출력 비트 열 전체를 0으로 만드는 일련의 논리 연산과 마스크를 제시하라.

XOR 1000 0001     
AND 1000 0001    

## 40번
```python
pattern = 0b10110101
mask1 = 0b10000001
pattern = pattern ^ mask1
mask2 = 0b10000001
print(bin(pattern & mask2))
```

## 41번
### a)
11010

### b)
00001111

### c)
010

### d)
001010

### e)
10000

## 42번
### a)
3F = 0011 1111

1100 1111

CF

### b)
0D = 0000 1101

0100 0011

43

### c)
FF = 1111 1111

1111 1111

FF

### d)
77 = 0111 0111

1101 1101

DD

## 43번
### a)
AB05

### b)
AB06

## 44번
> 비트들의 순서를 역으로 바꾸어주는 Vole 프로그램을 작성하라.

ABCD EFGH → HGFE DCBA
1. D와 H는 ROTATE1을 했을 때 목표 자리에 도달한다.
2. 1000 1000과 AND를 해서 D와 H의 비트를 살려준다.
3. C와 G는 ROTATE3을 했을 때 목표 자리에 도달한다.
4. 0100 0100과 AND를 해서 C와 G의 비트를 살려준다.
5. B와 F는 ROTATE5를 했을 때 목표 자리에 도달한다.
6. 0010 0010과 AND를 해서 B와 F의 비트를 살려준다.
7. A와 E는 ROTATE7을 했을 때 목표 자리에 도달한다.
8. 0001 0001과 AND를 해서 A와 E의 비트를 살려준다.
10. 전체 패턴들을 OR하여 합쳐준다.

118C : 셀8C LOAD    
A101 : 원본에서 ROTATE1    
2288 : 1000 1000    
8312 : 레지스터3 = 레지스터1 & 레지스터2    
A102 : 원본에서 ROTATE3    
2444 : 0100 0100    
8514 : 레지스터5 = 레지스터1 & 레지스터4    
A102 : 원본에서 ROTATE5    
2622 : 0010 0010     
8716 : 레지스터7 = 레지스터1 & 레지스터6      
A102 : 원본에서 ROTATE7     
2811 : 0001 0001    
8918 : 레지스터9 = 레지스터1 & 레지스터8    
7A35 : 레지스터A = 레지스터3 | 레지스터5   
7B79 : 레지스터B = 레지스터7 | 레지스터9   
7CAB : 레지스터C = 레지스터A | 레지스터B   
3C8C : 셀8C STORE

## 45번
> 주소 A2에 저장된 값에서 주소 A1에 저장된 값을 빼서 그 결과를 주소 A0에 넣는 Vole 프로그램을 작성하라.

11A2 : A2 LOAD    
12A1 : A1 LOAD    
2388 : 1111 1111    
9423 : A1 ^ 1111 1111 (보수 취함)    
2501 : 0000 0001     
5445 : 보수 취한 패턴에 +1    
5614 : 레지스터6 = A2 - A1     
36A0 : A0 STORE    

## 46번
30 * 1920 * 1080 * 24 = 1492992000bit

1492992000bps = 1492992Kbps = 1493Mbps = 1.5Gbps

USB 1.1(12Mbps) : 불가능    
USB 2.0(480Mbps) : 불가능   
USB 3.0(5Gbps) : 가능

## 47번
> 컴퓨터가 100만분의 1초에 500개의 명령을 실행한다면, 연속된 두 글자를 입력하는 사이에 몇 개의 명령을 실행할 수 있는가?

분당 200글자 입력  
글자당 0.3초 소요   

100만분의 1초에 500개 명령 = 1초에 500,000,000개 명령   
0.3초에 166,666,667개 명령

166,666,667개의 명령을 실행할 수 있다.

## 48번
분당 40 * 6 * 8 = 1920bit    
초당 1920 / 60 = 32bit

32bps

## 49번
00-01 11FE : 셀FE LOAD   
02-03 2001 : 레지스터0 = 0000 0001   
04-05 8210 : FE & 0000 0001   
06-07 B20A : 준비되었으면 0A로 JUMP    
08-09 B000 : 준비되지 않았으면 처음으로 JUMP   
0A-0B 35FF : 레지스터5 STORE    
0C-0D C000 : 종료

## 50번
00-01 20C1 : 레지스터0 = C1 (종료조건)   
02-03 2101 : 레지스터1 = 0000 0001   
04-05 2900 : 레지스터9 = 0x00   
06-07 1209 : 첫 주소(A0) LOAD (타겟 주소)   
08-09 39A0 : 셀A0~C0에 0x00 STORE (루프시작)   
0A-0B 5212 : 타겟 주소 = 현재 + 1    
0C-0D B212 : 타겟 주소가 C1이면 셀13(C000)으로 JUMP    
0E-0F 3209 : 타겟 주소를 다음 주소에 STORE    
10-11 B008 : 셀08(30XX)로 JUMP     
12-13 C000 : 종료

## 51번
200GB = 214,748,364,800Bytes = 1,717,986,918,400bit

15Mbps = 15,000Kbps = 15,000,000bps

114532.46sec = 31.8h

약 32시간

## 52번
250Kbps = 250,000bps

250,000 * 6.96 = 1,740,000bit

1,740,000개의 비트

## 53번
> 각기 100만분의 1초에 여러 자릿수를 갖는 숫자 두 개의 합을 계산할 수 있는 프로세서 32개를 갖고 있다고 가정하자.
> 64개의 숫자들에 대한 합을 100만분의 6초 만에 계산하기 위한 병렬 처리 방법을 기술하라.
> 한 개의 프로세서를 사용할 경우에 동일한 합의 계산에 필요한 시간은?

SIMD 구조로 덧셈을 수행한다.   
32개의 프로세서가 각각 숫자 2개를 더하여 16개의 결과값을 산출하고,   
그 결과값을 다시 16개의 프로세서가 2개씩 담당한 후 더해 8개의 결과값을 산출한다.

이런 식으로 결과값이 하나만 남을 때까지 덧셈을 반복하면,

64 → 32 → 16 → 8 → 4 → 2 → 1

위와 같이 총 여섯번의 덧셈이 일어나 100만분의 6초만에 모든 덧셈을 끝마치게 된다.

반면, 한 개의 프로세서를 사용한다면 동일한 작업에 100만분의 63초가 소요될 것이다.

## 54번
CISC = Complex Instruction Set Computer    
RISC = Reduced Instruction Set Computer

RISC는 가장 기본적인 명령들로만 구성하여 명령어의 개수를 줄인 CPU를 말하고,   
CISC는 프로그래밍을 돕기 위해 많은 수의 복잡한 명령들로 구성된 CPU를 말한다.

## 55번
> 처리율을 증가시키기 위한 두 가지 방식을 제시하라.

1. 파이프라이닝
2. 다중프로세싱

## 56번
> 여러 숫자들의 평균 계산에 있어 다중프로세서를 사용할 경우 어떻게 단일프로세서 컴퓨터를 사용할 경우보다 빨리 계산할 수 있는지 기술하라.

여러 숫자들의 평균을 구하려면 일단 모든 숫자의 합을 구해야 한다.  
이와 같은 덧셈을 처리하려면 (숫자개수-1)번 만큼의 덧셈 연산이 일어나야하는데,   
단일프로세서를 사용하는 경우 속절없이 모든 연산을 순서대로 진행할 수 밖에 없다.

반면, 다중프로세서를 사용하면 모든 프로세서가 동시에 숫자 두 개씩을 더한 후 그 결과값을 다시 더하는 방식으로    
여러개의 연산을 동시에 수행하여 총 소요시간을 대폭 줄일 수 있다.

## 57번
```python
import math

rad = float(input("원의 반지름 = "))
len = 2 * math.pi * rad       # 2πr
area = math.pi * (rad ** 2)       # πr²
print(f"원의 둘레 = {len}")
print(f"원의 넓이 = {area}")
```

## 58번
```python
str = input("문자열 = ")
times = int(input("횟수 = "))
print(str * times)
```

## 59번
```python
import math

side1 = float(input("Side 1 = "))
side2 = float(input("Side 2 = "))
hypo = math.sqrt(side1 ** 2 + side2 ** 2)
len = side1 + side2 + hypo
area = side1 * side2 / 2
print(f"빗변 = {hypo}")
print(f"둘레 = {len}")
print(f"넓이 = {area}")
```
