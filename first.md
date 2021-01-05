
# python 공부    

## 배열    

```python
word1 = " Welcome, "

print(word1[1:3])   # 1~2까지 출력
print(word1[:4])   # 0 ~ 4까지 출력
print(word1[5:])   # 5 ~ 출력

word2 = "my World !! "

word = word1 + word2  # 단어와 단어 +로 합치기 가능
                      # ,는 공백을 넣어 합치고 +는 공백없이 합쳐짐

print(word)           

# word에 'n'이 있는 지 찾기
print('n' in word) 
# word에 'e'이 있는지
print('e' in word) 

print(word1.lower())               #소문자 변환
print(word2.upper())               #대문자 변환
print(word.lstrip())               #왼쪽 공백 제거
print(word.rstrip())               #오른쪽 공백 제거
print(word.strip())                #오른쪽 왼쪽 제거
print(word.startswith(' Welcome')) #시작 문자열 확인
#print((word.lstrip).startswith('Welcome')) 오류가 나는 것을 확인
```

### .append
#### 배열을 크기를 정하지 않아도 append 함수로 배열 추가 가능
```python
a=[1,2,3]
print(a,type(a))
a.append('hello') 
print(a,type(a))
```
실행결과
```python
[1, 2, 3] <class 'list'>
[1, 2, 3, 'hello'] <class 'list'>
```
