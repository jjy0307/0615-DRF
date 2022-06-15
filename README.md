# 0615-DRF
Homework

 1. args, kwargs를 사용하는 예제 코드 짜보기
  def test(num1, num2, *args, **kwargs):
    print(f"num1 : {num1}")
    print(f"num2 : {num2}")
    print(args)
    print(kwargs)
    return

test(1,2,3,4,5,6,7,num3=8)

num1 : 1
num2 : 2
(3, 4, 5, 6, 7)
{'num3': 8}

 2. mutable과 immutable은 어떤 특성이 있고, 어떤 자료형이 어디에 해당하는지 서술하기
  변경가능한 객체(mutable) 과 변경불가능한 객체(immutable)
  변경가능한 객체 = List, Dict
  변경불가능한 객체 = Int, Str, Tuple

 3. DB Field에서 사용되는 Key 종류와 특징 서술하기
  FK : Foreign Key의 약자이며, 다른 테이블을 참조 할 때 사용
  UK : Unique key의 약자이며, 중복 값을 허용하지 않음
  PK : Primary Key의 약자이며, 테이블에서 반드시 존재해야 함
    PK는 두개 이상 존재 할 수 없고, UK와 마찬가지로 중복 값을 허용하지 않는다.
    Foreign Key를 사용할 경우 참조 할 테이블의 PK를 바라본다.

 4. django에서 queryset과 object는 어떻게 다른지 서술하기
  object = 단일 객체
  queryset = object의 list  객체들의 모음
