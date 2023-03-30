### byunlp

한국어 동사 자동 형태 변형기입니다.

'byunlp'는 과거형, 현재형, 현재진행형, 미래형, 사동표현, 주체 높임, 상대 높임, 부정형 변형을 지원합니다.

Automatic conjugation of Korean verb based on tense, voice, politeness and truth value.

'byunlp' enables Past, Present, Present Progressive, Future tense conjugations.

You can also passivize or make negation and honorifics. (Both Nominative and Relative honorifics)

Below is the distribution of python package 'byunlp'.

[https://pypi.org/manage/project/byunlp/releases/](https://pypi.org/manage/project/byunlp/releases/)

## **Overview**

- **conjugate.past()**: 과거형 반환
- **conjugate.present_progressive()**: 현재 진행형 반환
- **conjugate.future()**: 미래형 반환
- **conjugate.causative()**: 사동 형태 반환
- **conjugate.passive()**: 피동 형태 반환
- **conjugate.sangdae_honorific()**: 상대 높임 형태 반환
- **conjugate.subj_honorific()**: 주체 높임 형태 반환
- **conjugate.negation()**: 부정형 반환

## **Usage**

### **Installation**

You can install `byunlp` using `pip`:

```jsx
pip install byunlp
```

### **Requirements**

The following package is required when `byunlp`  is installed:

```jsx
pip install soynlp
```

## **Basic Usage**

Here is a simple example showing how to implement conjugation using `byunlp`:

```jsx
from byunlp import conjugate
```

```jsx
testset=['우회하다', '가다', '행선하다', '기어가다', '올라가다', '나가다', '따라가다', '뛰어가다', '되짚어가다', '잡혀가다'] 

for i in testset:
    print('{} -> {}'.format(i, conjugate.negation(i)))

```

### **Output**

```jsx
우회하다 -> ('우회하지 않다', '우회하지 못하다')
가다 -> ('가지 않다', '가지 못하다')
행선하다 -> ('행선하지 않다', '행선하지 못하다')
기어가다 -> ('기어가지 않다', '기어가지 못하다')
올라가다 -> ('올라가지 않다', '올라가지 못하다')
나가다 -> ('나가지 않다', '나가지 못하다')
따라가다 -> ('따라가지 않다', '따라가지 못하다')
뛰어가다 -> ('뛰어가지 않다', '뛰어가지 못하다')
되짚어가다 -> ('되짚어가지 않다', '되짚어가지 못하다')
잡혀가다 -> ('잡혀가지 않다', '잡혀가지 못하다')
데려가다 -> ('데려가지 않다', '데려가지 못하다')
찾아가다 -> ('찾아가지 않다', '찾아가지 못하다')
달려가다 -> ('달려가지 않다', '달려가지 못하다')
에워가다 -> ('에워가지 않다', '에워가지 못하다')
떠내려가다 -> ('떠내려가지 않다', '떠내려가지 못하다')
질러가다 -> ('질러가지 않다', '질러가지 못하다')
돌아서 지나가다 -> ('돌아서 지나가지 않다', '돌아서 지나가지 못하다')
```
