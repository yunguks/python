## file

#### \n 다음행으로 개행, 하나의 문자취급

```python
stuff = 'X\nY'
print(stuff)
X
Y
lens(stuff)   # 하나의 문자로 취급되어 len 3이 됨
3
```

#### handle = open(filename, mode)   
###### handle 은 파일 자체도 아니고 파일 안의 데이터도 아니다. 접근해주는 창구

```python
handle = open(filename, mode)

# 잘못된 파일명 예외처리
fname = input('Enter the file name: ')
try:
  fhand = open(fname)
except:
  print('File cannot be opende: ', fname)
  quit()  # 종료하는 함수 필수


# 파일을 열어 한줄 씩 출력
fhand = open('mbox.txt')
for cheese in fhand:
  cheese = cheese.retrip()  # 파일line 끝에 \n 개행 포함되어있어 제거
  print(cheese)             # print 끝에도 \n 개행 포함 중복


# 파일 모든정보를 한 문자열에 받기
fhand = open('mbox.txt')
one = fhand.read()   read() 읽기 메소드 호출


# 문자열 찾기
for line in fhand:
  line = line.retrip()
  if line.startswith('From:'):  # 첫단어가 From: 시작하는 문장 출력
    print(line)
  
  if not '@knu.ac.kr' in line:  # in함수로 특정단어가 포함된 line 찾기
    continue                    # 예외는 continue로 생략
  print(line)
  
  
    

```
