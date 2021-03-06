# 1단원 복습 문제

## 1번
### a)
1. (1, 0) → 0
2. (0, 1) → 0

### b)
1. (1, 0) → 0
2. (0, 1) → 1

### c)
1. (1, 0) → 0
2. (0, 1) → 1

## 2번
### a)
(0, 0) → 0   
(0, 1) → 0   
(1, 0) → 0   
(1, 1) → 1   

답은 AND연산이다.

### b)
(0, 0) → 0   
(0, 1) → 1   
(1, 0) → 1   
(1, 1) → 0

답은 XOR연산이다.

## 3번
### a)
#### 첫번째 펄스   
하 : 플립0→1 출력0→1   
상 : 플립1→0 출력0→0 (변화없음)   
출력 : (1, 0)

#### 두번째 펄스
하 : 플립0→1 출력1→0   
상 : 플립0→1 출력0→1  
출력 : (0, 1)

#### 세번째 펄스
하 : 플립0→1 출력0→1   
상 : 플립1→0 출력1→1 (변화없음)   
출력 : (1, 1)

#### 네번째 펄스
하 : 플립0→1 출력1→0   
상 : 플립0→1 출력1→0   
출력 : (0, 0)

### b)

A : 하 AND ~상    
B : ~하 AND 상   
C : 하 AND 상

#### 첫번째 클락 펄스   
하 : 플립0→1 출력0→1   
상 : 플립0→0 출력0→0 (변화없음)   
출력 : (1, 0)  
최종 출력 : (1, 0, 0)

#### 두번째 클락 펄스
하 : 플립0→1 출력1→0   
상 : 플립0→1 출력0→1  
출력 : (0, 1)  
최종 출력 : (0, 1, 0)

#### 세번째 클락 펄스
하 : 플립0→1 출력0→1   
상 : 플립1→0 출력1→1 (변화없음)   
출력 : (1, 1)  
최종 출력 : (0, 0, 1)

#### 네번째 클락 펄스
하 : 플립0→1 출력1→0   
상 : 플립0→1 출력1→0   
출력 : (0, 0)   
최종 출력 : (0, 0, 0)

이후로는 반복된다.

B에서 1이 나오는 클락 펄스 : 2, 6, 10번째  
C에서 1이 나오는 클락 펄스 : 3, 7, 11번째  
4번째 클락 펄스 : 어떤 출력에서도 1이 나오지 않는다.

## 4번
위쪽 입력이 순간적으로 0으로 바뀌면  
출력이 1이 되고, 0이 위쪽 AND게이트로 들어가므로 위쪽 입력이 1로 돌아가더라도 출력이 그대로 유지된다.  

아래쪽 입력이 순간적으로 0으로 바뀌면   
출력이 0이 되고, 0이 아래쪽 AND게이트로 들어가므로 아래쪽 입력이 1로 돌아가더라도 출력이 그대로 유지된다.   

<img src="https://user-images.githubusercontent.com/98504939/170405839-00ddaccd-cf1d-4574-b42e-0d2744d95e50.png" width=30%>

## 5번
00 02   
01 53  
02 01  
03 53

## 6번
두 자리 16진수의 크기는 1바이트다.  
따라서 256개까지의 셀이 존재할 수 있다.

네 자리 16진수의 크기는 2바이트이므로,  
이 경우에는 65536개까지의 셀이 존재할 수 있다.

## 7번
### a)
CD

답은 1100 1101이다.

### b)
67

답은 0110 0111이다.

### c)
9A

답은 1001 1010이다.

### d)
FF

답은 1111 1111이다.

### e)
10

답은 0001 0000이다.

## 8번
### a)
8F

1000 1111

답은 1이다.

### b)
FF

1111 1111

답은 1이다.

### c)
6F

0110 1111

답은 0이다.

### d)
1F

0001 1111

답은 0이다.

## 9번
### a)
1010 0000 1010

A 0 A

답은 A0A다.

### b)
1100 0111 1011

C 7 B

답은 C7B다.

### c)
0000 1011 1110

0 B E

답은 0BE다.

## 10번
하나의 픽셀을 표현하려면 3바이트가 필요하다. (R, G, B 각 1바이트 씩)  
1024 * 1024 * 3 = 3,145,728바이트 = 약 25.17MB (사진 1장 크기)  
256 / 25.17 = 10.17...   

최대 10장까지 저장할 수 있다.

## 11번
하나의 픽셀이 16비트, 즉 2바이트를 필요로 하는 경우다.  
1024 * 768 * 2 = 1,572,864바이트   

총 1,572,864개의 메모리 셀이 필요하다.

## 12번
### a)
> 자기디스크 저장장치에 비해 주기억장치가 갖는 장점 두 가지를 쓰라.
1. 기계적 동작을 요하지 않기 때문에 데이터를 읽고 쓰는 시간이 빠르다.
2. 기계적 고장을 일으킬 일이 없기 때문에 수명이 길다.

### b)
> 주기억장치에 비해 자기디스크 저장장치가 갖는 장점 두 가지를 쓰라.
1. 낮은 휘발성
2. 큰 저장 용량
3. 적은 비용

## 13번
합리적이지 않다.  
CD/DVD는 그정도 용량이 되지도 않고, 한번 저장한 데이터를 부분적으로 수정하는 것이 불가능하기 때문에  
하드디스크의 대체재로 적합하지 않다.

## 14번
100 * 50 * 2 = 10,000바이트  
10,000 / 1024 = 9.76...  

최소 10개의 섹터가 필요하다.

## 15번
ASCII는 8비트, 즉 1바이트다.  
3500 * 400 * 1 = 1,400,000바이트

ASCII를 사용한 경우, 1,400,000바이트가 필요하다.   
유니코드를 사용한 경우, 그 두 배인 2,800,000바이트가 필요하다.

## 16번
> 분당 3600번 회전하는 하드디스크 드라이브에서 대기시간은 얼마인가?

대기시간은 데이터 전송 요청과 데이터 수신 사이의 총 소요 시간을 말한다.  

분당 3600회 회전 = 초당 60회 회전 = 0.01666초당 1회 회전   
회전지연 = 0.01666초 / 2 = 0.00833초 = 8.3밀리초

대기시간 = 탐색시간 + 0.0083초(회전지연) + 요청 및 수신에 걸리는 시간

정확한 대기시간을 알 수 없는 거 아닌가?

## 17번
접근시간 = 탐색시간 + 회전지연

초당 360번 회전 = 0.002777초당 1회 회전   
회전지연 = 0.002777 / 2 = 0.001333초 = 1.3밀리초

평균접근시간 = 10밀리초 + 1.3밀리초 = 11.3밀리초

답은 11.3밀리초다.

## 18번
분당 60개의 단어  
한 단어는 다섯글자  
각 글자는 1바이트

60 * 5 * 1 = 300바이트

분당 300바이트 = 시간당 18000바이트 = 0.144MB   
640 / 0.144 = 4444.4444시간    
4444.4444 / 24 = 185.185일

최소 186일이 걸린다.

## 19번
57 68 61 74 20 64
6F 65 73 20 69 74
20 73 61 79 3F

W h a t (space) d o e s (space) i t (space) s a y ?

답은 What does it say?다.

## 20번
68 65 78 20 6E 6F 74 61 74 69 6F 6E

h e x (space) n o t a t i o n

답은 hex notation이다.

## 21번
### a)
Does 100/5=20?

01000100 01101111 01100101 01110011 00100000       
00110001 00110000 00110000 00101111 00111101 00110010 00110000 00111111

### b)
The total cost is $7.25.

01010100 01101000 01100101 00100000     
01110100 01101111 01110100 01100001 01101100 00100000      
01100011 01101111 01110011 01110100 00100000         
01101001 01110011 00100000     
00100100 00110111 00101110 00110010 00110101 00101110 

## 22번
### a)
01000100 01101111 01100101 01110011 00100000     
00110001 00110000 00110000 00101111 00111101 00110010 00110000 00111111

44 6F 65 73 20
31 30 30 2F 3D 32 30 3F

### b)
01010100 01101000 01100101 00100000      
01110100 01101111 01110100 01100001 01101100 00100000      
01100011 01101111 01110011 01110100 00100000         
01101001 01110011 00100000     
00100100 00110111 00101110 00110010 00110101 00101110 

54 68 65 20     
74 6F 74 61 6C 20     
63 6F 73 74 20      
69 73 20       
24 37 2E 32 35 2E

## 23번
8 1000   
9 1001   
10 1010   
11 1011   
12 1100   
13 1101   
14 1110   
15 1111   
16 10000   
17 10001   
18 10010  

## 24번
### a)
23

00110010 00110011

### b)
23

10111

## 25번
> 2진법 표현에서 비트들 중 한 개만이 1인 숫자들에는 어떤 것들이 있는가?
> 이러한 성질을 갖는 값 중에 가장 작은 것 6개만 나열하라.

음... 뭘 구하라는건지 모르겠다.  
분수, 2의보수, 부동소수점, 초과표기법 이런 애들 중에 1이 하나만 있으면서 가장 작은 경우를 물어보는건가?


## 26번
### a)
111

답은 7이다.

### b)
0001

답은 1이다.

### c)
10101

답은 21이다.

### d)
1000

답은 8이다.

### e)
10011

답은 19다.

### f)
000000

답은 0이다.

### g)
1001

답은 9다.

### h)
10001

답은 17이다.

### i)
100001

답은 33이다.

### j)
11001

답은 25다.

### k)
11010

답은 26이다.

### l)
11011

답은 27이다.

## 27번
### a)
7

답은 111이다.

### b)
11

답은 1011이다.

### c)
16

답은 10000이다.

### d)
17

답은 10001이다.

### e)
31

답은 11111이다.

## 28번
### a)
10001

답은 1이다.

### b)
10101

답은 5다.

### c)
01101

답은 -3이다. 

### d)
01111

답은 -1이다.

### e)
11111

답은 15다.

## 29번
### a)
0

답은 100이다.

### b)
3

답은 111이다.

### c)
-2

답은 010이다.

### d)
-1

답은 011이다.

### e)
2

답은 110이다.

## 30번
### a)
01111

답은 15다.

### b)
10100

답은 -12다.

### c)
01100

답은 12다.

### d)
10000

답은 -16이다.

### e)
10110

답은 -10이다.

## 31번
### a)
13

답은 0001101이다.

### b)
-13

답은 1110011이다.

### c)
-1

답은 1111111이다.

### d)
0

답은 0000000이다.

### e)
16

답은 0010000이다.

## 32번
### a)
00101 + 01000

답은 01101이다.

### b)
11111 + 00001

답은 00000이다. 

### c)
01111 + 00001

답은 10000이다.  
오버플로가 발생하여 답이 올바르지 않다.

### d)
10111 + 11010

답은 10001이다.

### e)
11111 + 11111

답은 11110이다.

### f)
00111 + 01100

답은 10011이다.  
오버플로가 발생하여 답이 올바르지 않다.

## 33번
### a)
5 + 1 = 6

00101 + 00001 = 00110 = 6

답이 일치한다.

### b)
5 - 1 = 4

00101 - 00001 = 00101 + 11111 = 00100 = 4

답이 일치한다.

### c)
12 - 5 = 7

01100 - 00101 = 01100 + 11011 = 00111 = 7

답이 일치한다.

### d)
8 - 7 = 1

01000 - 00111 = 01000 + 11001 = 00001 = 1

답이 일치한다.

### e)
12 + 5 = 17

01100 + 00101 = 10001 = -15

오버플로가 발생하여 답이 일치하지 않는다.

### f)
5 - 11 = -6

00101 - 01011 = 00101 + 10101 = 11010 = -6

답이 일치한다.

## 34번
### a)
11.11

답은 3과 4분의 3이다.

### b)
100.0101

답은 4와 16분의 5다.

### c)
0.1101

답은 16분의 13이다.

### d)
1.0

답은 1이다.

### e)
10.01

답은 2와 4분의 1이다.

## 35번
### a)
5와 4분의 3

### b)
15와 16분의 15

답은 1111.1111이다.

### c)
5와 8분의 3

답은 101.011이다.

### d)
1과 4분의 1

답은 1.01이다.

### e)
6과 8분의 5

답은 110.101이다.

## 36번
### a)
0 101 1001

답은 1.001이다.

### b)
1 100 1000

답은 -0.1000이다.

### c)
1 010 1100

답은 -0.0011이다.

### d)
0 011 1001

답은 0.01001이다.

## 37번
### a)
-(7과 2분의 1) = -111.1

답은 1 111 1111이다.

### b)
2분의 1 = 0.1

답은 0 100 1000이다.

### c)
-(3과 4분의 3) = -11.11

답은 1 110 1111이다.

### d)
32분의 7 = 0.00111

답은 0 010 1110이다.

### e)
32분의 31 = 0.11111

답은 0 100 1111이다. (절삭오차 32분의 1)

## 38번
8분의 3 = 0.011

0 101 0011    
0 100 0110    
0 011 1100

## 39번

### 2의 멱승을 분모로 갖는 분수로 변환하여 접근
2의 제곱근 = 1.414(10진법) = 1과 1000분의 414   
= 1과 1024분의 424 = 1과 256분의 106 = 1과 128분의 53

1과 128분의 53 = 1.0110101(2진법)   
0 101 1011 = 1.011 (절삭오차 128분의 5)

가장 가까운 값은 1.011(2진법)이다.  
이 값은 10진법으로 1과 8분의 3이다. = 1.375
따라서, 이 값을 제곱했을 때 실제 얻게 되는 값은 1.890625다.

### 10진수→2진수 소수부 변환법으로 접근
소수부에 2를 곱해 결과의 정수부를 기록하고 소수부만 남긴 후 다시 2를 곱한다.  
소수부가 0이 될 때까지 반복하고, 변환이 끝나면 기록해둔 정수부를 순서대로 읽는다.  

이 방법을 사용해 1.4142를 2진수로 변환하면 1.011010... 무한소수가 나온다.  
(대부분의 10진수 유한소수는 2진수 무한소수로 변환된다.)  

이 경우에도 8비트 부동소수점 형식을 사용하면 1.011까지만 표현할 수 있다.  

## 40번

### 2의 멱승을 분모로 갖는 분수로 변환하여 접근
10분의 1 = 약 32분의 3 = 0.00011(2진법)  

가장 가까운 값은 0 001 1100이다. (10진법 0.09375)

### 10진수→2진수 소수부 변환법으로 접근
0.000110011...  

8비트 부동소수점을 사용하면 0.00011까지만 표현할 수 있다.                                                        

## 41번
미터 단위계를 사용하여 측정값들을 부동소수점 표기법으로 기록할 경우,  
유효숫자 부분의 자릿수가 부족하여 저장될 값의 일부를 잃어버릴 수 있다. (= 절삭오차)

예를 들어, 110cm를 미터 단위로 기록할 경우, 2진법 근사값은 1.000110...m다.   
8비트 부동소수점을 사용하면 1.000m까지만 기록이 가능하므로 그 밑으로는 절삭오차가 발생한다.

## 42번
01011 11011  
하나는 16 초과 표기법, 하나는 2의 보수 표기법 (둘은 같은 값)

### a)
#### 전자가 16 초과 표기법, 후자가 2의 보수 표기법인 경우
전자 : 11 - 16 = -5  
후자 : -5  
이 경우, 두 수는 -5다.

#### 전자가 2의 보수 표기법, 후자가 16 초과 표기법인 경우
전자 : 11   
후자 : 27 - 16 = 11   
이 경우, 두 수는 11이다.

### b)
최상위 비트를 제외한 모든 비트가 동일하다.

## 43번
1번 1000 0010  
2번 0110 1000  
3번 0000 0010

1번과 3번은 최상위 비트를 제외한 모든 비트가 동일하다.  
따라서 두 비트 패턴 중에 초과 표기법과 2의 보수 표기법을 따르는 패턴이 존재할 것임을 추정할 수 있다.  

즉, 2번이 8비트 부동소수점 형식을 따르고 있음을 알 수 있다.   
해석해보면, 2번이 나타내는 수는 10이다.

1번과 3번도 10을 나타내고 있어야하므로  
1번은 초과 표기법을, 3번은 2의 보수 표기법을 따르고 있음을 알 수 있다.

1번 : 초과 표기법  
2번 : 8비트 부동소수점 형식  
3번 : 2의 보수 표기법  
공통적으로 표현하는 값 : 10

## 44번

### a)
6과 2분의 1 = 6.1

정확히 표현된다.

### b)
16분의 13 = 0.1101

정확히 표현된다.

### c)
9 = 1001

정확히 표현된다.

### d)
32분의 17 = 0.10001

유효숫자 부분의 자릿수를 초과하므로 정확히 표현될 수 없다.

### e)
16분의 15 = 0.1111

정확히 표현된다.

## 45번
4비트 : 16개 (0\~15)  
6비트 : 64개 (0\~63)

표현할 수 있는 최대값이 48만큼 커진다.  

2의 보수를 사용할 경우의 표현 범위는 다음과 같다.

4비트 : 16개 (-8\~7)  
6비트 : 64개 (-32\~31)

표현할 수 있는 최소값이 24만큼 작아지며,  
표현할 수 있는 최대값도 24만큼 커진다.

## 46번
4MB = 4,194,304바이트

총 4,194,304개의 주소가 존재하고,  
4,194,304는 2의 22승이므로 모든 주소는 22비트로 표현이 가능하다.

가장 큰 주소는 0011 1111 1111 1111 1111일 것이고,  
이를 16진수로 표현하면 3 F F F F다.

답은 3FFFF다.

## 47번
xxy yyx xxy xxy yyx

112 3 221 3 4 3 4 3 5

답은 1123221343435다.

## 48번
22123113431213536

yyxy xx yyxy xyx xx xyx

답은 yyxy xx yyxy xyx xx xyx다.

## 49번
xxy yyx xxy xxyy

답은 [x, y, 공백, xxy, yyx, xxyy]다.

## 50번
MPEG 기법을 사용할 경우,   
40Mbps의 전송속도를 제공하는 통신경로 상에서 비디오가 성공적으로 재생되므로 57.6bps로는 역부족이다.

## 51번
### a)
Does 100/5=20?

001000100 001101111 001100101 101110011 100100000       
100110001 000110000 000110000 100101111 100111101 100110010 000110000 000111111

### b)
The total cost is $7.25.

101010100 101101000 001100101 100100000     
001110100 001101111 001110100 101100001 001101100 100100000      
001100011 001101111 101110011 001110100 100100000         
001101001 101110011 100100000     
000100100 100110111 000101110 100110010 000110101 000101110 

## 52번
11001 11011 10110 00000 11111   
10001 10101 00100 01110

오류가 발생한 비트 열은 11011, 00000, 10001이다.  
(짝수 개의 오류가 발생한 비트 열은 탐지할 수 없다.)

## 53번
동일한 패턴이 반복되므로 오류가 발생했을 시 패턴끼리 대조하여 정상 데이터로 조정할 수 있다.

## 54번
### a)
111010 110110

H E

답은 HE다.

### b)
101000 100110 001100

F E D

답은 FED다.

### c)
011101 000110 000000 010100

D E A D

답은 DEAD다.

### d)
010010 001000 001110 101111 000000 110111 100110

C A B B A G E

답은 CABBAGE다.

### e)
010011 000000 101001 100110

C A F E

답은 CAFE다.

## 55번
```python
USD_to_GBP = 0.79
USD_to_EUR = 0.93
USD_to_JPY = 126.77

GBP_sign = "\u00A3"
EUR_sign = "\u20AC"
JPY_sign = "\u00A5"

dollars = 1000

pounds = dollars * USD_to_GBP
euros = dollars * USD_to_EUR
yen = dollars * USD_to_JPY

print(f"Today, ${dollars}")
print(f"converts to {GBP_sign}{pounds}")
print(f"converts to {EUR_sign}{euros}")
print(f"converts to {JPY_sign}{yen}")
```
```
Today, $1000
converts to £790.0
converts to €930.0
converts to ¥126770.0
```

## 56번
```python
USD_to_GBP = 0.79
USD_to_EUR = 0.93
USD_to_JPY = 126.77
USD_to_KOR = 1265.5

GBP_sign = "\u00A3"
EUR_sign = "\u20AC"
JPY_sign = "\u00A5"
KOR_sign = "\u20A9"

dollars = 1000

pounds = dollars * USD_to_GBP
euros = dollars * USD_to_EUR
yen = dollars * USD_to_JPY
won = dollars * USD_to_KOR

print(f"Today, ${dollars}")
print(f"converts to {GBP_sign}{pounds}")
print(f"converts to {EUR_sign}{euros}")
print(f"converts to {JPY_sign}{yen}")
print(f"converts to {KOR_sign}{won}")
```
```
Today, $1000
converts to £790.0
converts to €930.0
converts to ¥126770.0        
converts to ₩1265500.0
```

## 57번
```python
USD_to_GBP = 0.79
USD_to_EUR = 0.93
USD_to_JPY = 126.77
USD_to_KOR = 1265.5

dollars = 1000

pounds = dollars * USD_to_GBP
euros = dollars * USD_to_EUR
yen = dollars * USD_to_JPY
won = dollars * USD_to_KOR

print(f"Today, ${dollars}")
print(f"converts to £{pounds}")
print(f"converts to €{euros}")
print(f"converts to ¥{yen}")
print(f"converts to ₩{won}")
```
```
Today, $1000
converts to £790.0
converts to €930.0
converts to ¥126770.0
converts to ₩1265500.0
```

## 58번
코드의 변경이 간편해진다.   
환전할 금액을 변경하고 싶을 시 dollars에 담긴 값만 바꿔주면    
dollars가 쓰이는 모든 곳에서 금액이 일괄 변경되는 효과를 누릴 수 있다.

## 59번
```python
b = 12345678

kb = b / 1024
mb = kb / 1024
gb = mb / 1024

print(f"Bytes = {b}")
print(f"KiloBytes = {kb}")
print(f"MegaBytes = {mb}")
print(f"GigaBytes = {gb}")
```
```
Bytes = 12345678
KiloBytes = 12056.326171875
MegaBytes = 11.77375602722168
GigaBytes = 0.011497808620333672
```

## 60번
```python
sec_per_music = 180
stereo_size = 180 * 44100 * 32
print(f"Stereo Size = {stereo_size}bits")
```
```
Stereo Size = 254016000bits
```

## 61번
```python
days_per_year = days_per_week ** weeks_per_year     # 이 부분이 틀렸다!
```
`**`는 제곱을 구하는 기호다.  
여기서는 `*`를 사용해 단순 곱을 구하여야 한다.
