# 핵심

이 문제에서 가장 핵심은 '**최빈값** 구하기' 이다.

- vector를 쓰거나, round()를 쓰거나, sort()를 쓰거나, 최빈값 플래그를 쓰는 것은 일단 '구현 실력' 문제이다.

- 제일 중요하게 봐야할 부분은 '최빈값'을 구하는 부분인데, 단순하게 접근해서 하다가는 시간 초과나기 십상이다.
  
- 문제에서 두는 '제한'을 잘 보자. (hint!)
  - 절댓값 4000 이하로 제한하고 있다.
  - '빈도' 를 저장할 `-4000 ~ 4000` 범위의 배열을 미리 정의해놔도 메모리가 충분하다! (성능은 당연히 좋고)

## 개선할 문제

main() 함수에서 스택을 너무 많이쓰고 있으니 힙 메모리로 데이터를 좀 옮기라는 경고가 뜬다.
- 어떻게 해결할까?
- `int count[8001]` 대신 `std::vector`를 써보자?

