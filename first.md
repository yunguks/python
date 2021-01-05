
# python 공부    

## 배열    

```python
word1 = " Welcome, "


print(word1[1:3])   # 1~2까지 출력

print(word1[:4])   # 0 ~ 4까지 출력

print(word1[5:])   # 5 ~ 출력

word2 = "my World !! "

word = word1 + word2

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
