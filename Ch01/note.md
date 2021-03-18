## 구성
```
01-method : instance/class/static method
02-list-comprehension : map/filter 대신 리스트 컴프리헨션
```
## 반드시 따를 PEP 8
### 화이트스페이스 - 코드의 명료성에 영향
+ 탭이 아닌 스페이스로 들여쓰기
+ 문법적으로 의미있는 들여쓰기는 각 수준마다 스페이스 네 개
+ 한 줄의 문자 길이가 79자 이하
+ 표현식이 길어 다음줄로 이어지면 일반적인 들여쓰기 수준에 추가로 스페이스 네 개 사용
+ 파일에서 함수와 클래스는 빈 줄 두 개로 구분
+ 클래스에서 메서드는 빈 줄 하나로 구분
```
def sample_func():
    sample_instance = ''
    pass
    

Class CapitalizedWord:
    
    def __init__(self):
        self._leading_underscore = '' # 보호 인스턴스
        self.__double_leading_underscore = '' # 비공개 인스턴스 속성
    
    def lowercase_underscore():
        pass


## 모듈수준의 상수
#ALL_CAPS 형식
```
### 표현식과 문장
```
# 인라인 부정
if not a is b (x)
if a is not b (o)
# 빈 값, true/false
if x == '': (x)
if x: (o)
```
+ 모듈 임포트시 절대 이름 사용
+ 표준 라이브러리 모듈 -> 서드파티 모듈 -> 자신이 만든 모듈 순서 - 각각 알파벳 순서
#### 표현식이 복잡해지기 시작하면 작은 조각으로 분할하고 로직을 헬퍼함수로 옮기기
+ 코드의 간결성 < 명확성
