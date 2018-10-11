# 181011

## for문  
형식 :   
<pre>for i in range(1, 11, 1) :   
   hap = hap + i </pre>  
i는 1부터 시작해서 < 11까지 반복한다. 다른 언어들 처럼 <=는 사용 못한다.  

## 문자열의 한 글자씩 접근 방법  
<pre>str = "abc"
print(str[0])
print(str[1])
print(str[2])</pre>  
<pre>a
b
c</pre>  
str을 한 배열로 생각한다.  

## 하트 만들기  
<pre>## 변수 선언 부분
i, k, heartNum = 0, 0, 0
numStr, ch, heartStr = "", "", ""

##메인(main) 코드 부분
numStr = input("숫자를 여러 개 입력하세요 : ")
print("")

i = 0
ch = numStr[i]
while True :
    heartNum = int(ch)

    heartStr = ""
    for k in range (0, heartNum) :
        heartStr += "\u2665"  ##\u2665 = 하트문자
        k += 1

    print(heartStr)

    i += 1
    if(i > len(numStr) - 1) :
        break

    ch = numStr[i]</pre>
    
여기서 \u2665는 하트 문자를 나타낸다. \(백슬래쉬)뒤에 어떤 숫자를 쓰느냐에 따라서 다른 문자를 나타낼 수 있다.
