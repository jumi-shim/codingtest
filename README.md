# codingtest

## programmers
- [주식 가격](https://programmers.co.kr/learn/courses/30/lessons/42584) level2 ☆  
  스택/큐 카테고리에 있는 문제여서 바로 아 스택을 이용해야겠다 생각했지만 그게 아니였다면 스택을 바로 생각하기는 어려웠을 것같다. 아마 그냥 중첩 반복문 돌리면서 계산하였을 것이다.  
  가격과 순서(인덱스)를 차례대로 스택에 push하고 만약 제일 위에 있는 수 보다 작은 수를 넣어야 하면 pop을 하여 인덱스로 시간을 구하는 방식으로 하였다.  
  숫자를 탐색하면서 특정 조건에 어떤 로직을 쓰고 싶을 때는 스택의 성질을 이용하면 편리하다는 점을 알았다.
- [소수 찾기](https://programmers.co.kr/learn/courses/30/lessons/42839) level2 ☆  
  순열을 이용해서 모든 경우의 수를 소수판별을 하여 구했다. 에라토스테네스의 체 + 집합을 이용하여 구하는 풀이도 있었다.  
  에라토스테네스의 체는 범위에서 합성수를 지우는 방식으로 소수를 구한다. 0, 1은 지우고 지워지지 않는 제일 작은 수 2를 소수 채택하고 2의 배수를 모두 지우고 지워지지 않는 제일 작은 수 3을 소수로 채택하고.. ~ 이런 방식으로 범위 안에서 소수를 구하는 방식이다.
- [메뉴 리뉴얼](https://programmers.co.kr/learn/courses/30/lessons/72411) level2 ☆☆  
  처음에 접근했던 방식은 orders에 있는 총 메뉴들을 course로 조합을 구했다. 구한 조합으로 orders에 있는 각 주문들에 조합이 포함되는지 확인하는 방법이었다. 시간초과가 났다...!  
  하지만.. 생각을 바꾸면.. 각 order 마다 course로 조합을 구해 딕셔너리에 저장하고, 만약 똑같은 조합이 나온다면 +1 증가시켜주어 해당 course에 대한 조합 정보를 구한다. 그 후 가장 많이 나온 경우를 결과에 저장하면 끝.  
  프로그래머스 점수를 보니 어려운 사람들에게 어려운 문제는 아니였던 것같다. 하지만 처음 생각한 방식에 사로잡힌 나는.. 꽤 오래 걸렸다.. 😩  
  🖍결국, 1번 방법은 총 조합의 경우를 구하고 각 order마다 총 조합에서 어떤 것이 해당되는지 확인하는 절차가 있었고 2번 방법은 1개마다 조합을 구하고 그 결과를 누적 저장한다. 그러니 1번에서 했던 확인 절차를 안 해도 되는 것이다!!!! 게다가, 문제는 결국 가장 많이 나오는 경우를 원하기 때문에 더더욱 2번이 효율적인 것이다.  
  문제를 풀었는데 시간초과가 났으면 다른 방식을 생각해보아야 하는데 항상 이 부분이 어려운 것같다.
- [프렌즈4블록](https://programmers.co.kr/learn/courses/30/lessons/17679#) level2 ☆☆  
  블록을 내리는 부분에서 시간이 오래 걸렸다.. 쉬워보이는데 은근 어려웠다. 일반화를 하고 풀기 위한 생각 정리가 중요함을 느꼈더 문제! 예시에서 나오는 것이 다가 아니라 문제를 읽고 일반화 + 예외까지 생각하는 과정을 배웠던 문제!  
- [네트워크](https://programmers.co.kr/learn/courses/30/lessons/43162) level3 ☆☆  
  오랜만에 다시 dfs를 공부하고 문제를 풀었다. 역시 여러번 공부하면 쉬워지는 것이 맞나보다. dfs로 그래프 탐색을 한번에(한 줄 그리기??) 할 수 있으면 네트워크 1개인 것이다. 문제를 읽고 dfs를 생각하는 재미있는 문제~!~!
