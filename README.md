# codingtest

## programmers
- [주식 가격](https://programmers.co.kr/learn/courses/30/lessons/42584) level2️⃣ ⭐️  
  스택/큐 카테고리에 있는 문제여서 바로 아 스택을 이용해야겠다 생각했지만 그게 아니였다면 스택을 바로 생각하기는 어려웠을 것같다. 아마 그냥 중첩 반복문 돌리면서 계산하였을 것이다.  
  가격과 순서(인덱스)를 차례대로 스택에 push하고 만약 제일 위에 있는 수 보다 작은 수를 넣어야 하면 pop을 하여 인덱스로 시간을 구하는 방식으로 하였다.  
  숫자를 탐색하면서 특정 조건에 어떤 로직을 쓰고 싶을 때는 스택의 성질을 이용하면 편리하다는 점을 알았다.
- [소수 찾기](https://programmers.co.kr/learn/courses/30/lessons/42839) level2️⃣ ⭐️  
  순열을 이용해서 모든 경우의 수를 소수판별을 하여 구했다. 에라토스테네스의 체 + 집합을 이용하여 구하는 풀이도 있었다.  
  에라토스테네스의 체는 범위에서 합성수를 지우는 방식으로 소수를 구한다. 0, 1은 지우고 지워지지 않는 제일 작은 수 2를 소수 채택하고 2의 배수를 모두 지우고 지워지지 않는 제일 작은 수 3을 소수로 채택하고.. ~ 이런 방식으로 범위 안에서 소수를 구하는 방식이다.
- [메뉴 리뉴얼](https://programmers.co.kr/learn/courses/30/lessons/72411) level2️⃣ ⭐️⭐️  
  처음에 접근했던 방식은 orders에 있는 총 메뉴들을 course로 조합을 구했다. 구한 조합으로 orders에 있는 각 주문들에 조합이 포함되는지 확인하는 방법이었다. 시간초과가 났다...!  
  하지만.. 생각을 바꾸면.. 각 order 마다 course로 조합을 구해 딕셔너리에 저장하고, 만약 똑같은 조합이 나온다면 +1 증가시켜주어 해당 course에 대한 조합 정보를 구한다. 그 후 가장 많이 나온 경우를 결과에 저장하면 끝.  
  프로그래머스 점수를 보니 어려운 사람들에게 어려운 문제는 아니였던 것같다. 하지만 처음 생각한 방식에 사로잡힌 나는.. 꽤 오래 걸렸다.. 😩  
  🖍결국, 1번 방법은 총 조합의 경우를 구하고 각 order마다 총 조합에서 어떤 것이 해당되는지 확인하는 절차가 있었고 2번 방법은 1개마다 조합을 구하고 그 결과를 누적 저장한다. 그러니 1번에서 했던 확인 절차를 안 해도 되는 것이다!!!! 게다가, 문제는 결국 가장 많이 나오는 경우를 원하기 때문에 더더욱 2번이 효율적인 것이다.  
  문제를 풀었는데 시간초과가 났으면 다른 방식을 생각해보아야 하는데 항상 이 부분이 어려운 것같다.
- [프렌즈4블록](https://programmers.co.kr/learn/courses/30/lessons/17679#) level2️⃣ ⭐️⭐️  
  블록을 내리는 부분에서 시간이 오래 걸렸다.. 쉬워보이는데 은근 어려웠다. 일반화를 하고 풀기 위한 생각 정리가 중요함을 느꼈더 문제! 예시에서 나오는 것이 다가 아니라 문제를 읽고 일반화 + 예외까지 생각하는 과정을 배웠던 문제!  
- [네트워크](https://programmers.co.kr/learn/courses/30/lessons/43162) level3️⃣ ⭐️⭐️  
  오랜만에 다시 dfs를 공부하고 문제를 풀었다. 역시 여러번 공부하면 쉬워지는 것이 맞나보다. dfs로 그래프 탐색을 한번에(한 줄 그리기??) 할 수 있으면 네트워크 1개인 것이다. 문제를 읽고 dfs를 생각하는 재미있는 문제~!~!
- [가장 큰 정사각형 찾기](https://programmers.co.kr/learn/courses/30/lessons/12905) level2️⃣ ⭐️⭐️  
  처음에는 board 확인을 여러번 하는 방식으로(4중첩 반복문..) 하였다. 예상대로 시간초과가 났고 그래프를 1번만 탐색하면서 확인하는 방법을 모르겠어서 다른 사람들의 풀이를 보았다. 다이나믹 프로그래밍 방법을 이용했다.  
  다이나믹 프로그래밍의 핵심은 큰 문제를 작은 문제로 나눌 수 있는지이다. 여기서는 (1,1)부터 주변에((-1,0),(0,-1),(-1,-1))0이 있는지 확인해 나간다. 주변 값들 중에 최소값을 해당 위치에 더해서 기록을 하는데 이때 주변에 0이 있다면 값은 그대로이고 그게 아니라면 해당 값은 해당 지점에서 왼쪽 상단 방향으로 가장 큰 사각형의 길이이다...!
- [땅따먹기](https://programmers.co.kr/learn/courses/30/lessons/12913) level2️⃣ ⭐️⭐️  
  이 문제는 당장 최선의 선택을 하면 최종 결과가 최선의 결과인지 모른다. 이것처럼 지금 선택이 다음의 선택에 영향을 미칠 때..! 이런 경우에는 그냥 모든 경우의 수를 저장하면 편리하다.(왜 이런 생각을 못했지..??? 최종 값을 구하기 위해 관려 없어 보이는 다른 값들을 구하면서(이용하면서) 코드를 작성하면 편리한 경우였다. 무작정 내가 원하는 특정 값만! 구하려고 하지말고~) 다이나믹 프로그래밍이라고 생각 가능하다. 아직 많이 부족한듯..
- [다음 큰 숫자](https://programmers.co.kr/learn/courses/30/lessons/12911) level2️⃣ ⭐️  
  이진수를 구할 때 반복문으로 직접 구했는데 이 방법 말고 String(n, radix: 2)를 이용하는 방법이 있었고, nonzeroBitCount를 이용하여 이진수의 1의 개수를 구하는 방법이 있다.
- [JadenCase 문자열 만들기](https://programmers.co.kr/learn/courses/30/lessons/12951) level2️⃣ ⭐️  
  문자열 관련 함수를 정리해야겠다! 스위프트는 문자열 다루기가 상대적으로 까다로워서 배열로 바꿔 푸니까 해결쓰~!
- [올바른 괄호](https://programmers.co.kr/learn/courses/30/lessons/12909) level2️⃣ ⭐️  
  너무 흔한 유형이라서 빠르게 풀 수 있었다. 차례대로 탐색할 때 특정 조건에 부합하는지 확인 할 때 스택을 이용할 수 있다.
- [[3차] n진수 게임](https://programmers.co.kr/learn/courses/30/lessons/17687) level2️⃣ ⭐️  
  숫자 하나하나 증가시켜 주면서 조건을 반영하는 변수를 적절하게 초기화를 잘 해줘야 하는 문제였다! 나는 숫자를 하나하나 구하면서 필요한 수를 저장했다면 다른 사람은 일단 모든 수를 다 저장하고 마지막에 원하는 숫자만 저장하는 방식으로 한 사람도 있었다. 후자의 방법이 변수 초기화 실수를 안 할 가능성이 높기 때문에 좋은 것같다.
- [신고 결과 받기](https://programmers.co.kr/learn/courses/30/lessons/92334?language=swift) level1️⃣ ⭐️
  딕셔너리의 value의 형태가 배열이길 원했다. key를 만들어주고 그 key로 접근하여 dic[key].append(a) 이런식으로 했을 때 오류가 났다. 여기서 안전성을 중요시하는 스위프트의 특성을 느낄 수 있었는데 key값이 있는지 모르니, append함수를 쓰니까 오류가 난 것..! 옵셔널 처리를 잘 해줘야 한다. key가 dic에 있는게 확실하다면 dic[key]!.append(a) 하면 오류가 나지 않는다.
- [큰 수 만들기](https://programmers.co.kr/learn/courses/30/lessons/42883#) level2️⃣ ⭐️⭐️  
처음에는 조합을 이용해서 모든 경우의 수를 다 따져보는 쪽으로 밖에 아이디어가 떠오르지 않았다. 어쩔 때는 무식한 방법이 최선일 때도 있지만 이 문제는 아니였다. 조금만 더 생각을 해 보면 가장 큰 수를 만들기 위해서는 뒤에 오는 숫자는 앞에 있는 숫자보다 작아야 한다. -> 엇?? 이거는 스택으로 편하게 구할 수 있는데??!😆 홧팅 .. 
