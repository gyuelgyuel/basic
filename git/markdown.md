> markdown 사용법 정리

# 제목과 목차
```markdown
# 제목
## 중제목
### 소제목
---
```
#, ##, ###을 이용하여 제목과 내용 분리 (---는 마지막)

```markdown
1. 첫번째 항목
2. 두번째 항목
3. 세번째 항목

-python
-HTML
-css
-Django
```
ordered system, unordered system은 다음과 같이 표시


# 글씨체와 내용칸
```markdown
*itatlian*
**bold**
```
기울임체와 굵음은 위와 같이 표시

```markdown
파이썬출력은 `print()`
```
` backtick 기호를 통해 명령 관련 표시

```markdown
> 강조하는 line
```
줄 강조는 줄의 앞에 > 입력

```markdown
"```python
print()
```"
"```javascript
console.log('hello')
```"
```
명령어를 코딩언어의 문법에 맞추어 표시를 할 경우 위의 " 를 제외하고 입력


## 링크 & 이미지
```markdown
[address_name](address)
[image_name](image_address)
```
링크와 이미지는 링크의 이름, 이미지의 이름을 각각 대괄호 안에 넣고, 실제 주소를 괄호안에 입력
아래는 구글 링크와 구글 이미지 적용 예시이다.

[google](https://google.com)
![googleimage](https://upload.wikimedia.org/wikipedia/commons/thumb/2/2f/Google_2015_logo.svg/1280px-Google_2015_logo.svg.png)


# 표
```
| 이름 | 주소 |
| --- | --- |
| 홍길동 | 서울 |
| 이순신 | 대전 |
```
|로 구분할 경우 아래와 같이 표로 표시
| 이름 | 주소 |
| --- | --- |
| 홍길동 | 서울 |
| 이순신 | 대전 |

