# java

### 문제 설명
문자열 s를 숫자로 변환한 결과를 반환하는 함수, solution을 완성하세요.

제한 조건
1. s의 길이는 1 이상 5이하입니다.
2. s의 맨앞에는 부호(+, -)가 올 수 있습니다.
3. s는 부호와 숫자로만 이루어져있습니다.
4. s는 "0"으로 시작하지 않습니다.


입출력 예

- 예를들어 str이 "1234"이면 1234를 반환하고, "-1234"이면 -1234를 반환하면 됩니다.
- str은 부호(+,-)와 숫자로만 구성되어 있고, 잘못된 값이 입력되는 경우는 없습니다.


#### Solution.java
------------------------------------------------
class Solution {
    public int solution(String s) {
        
        int answer = Integer.parseInt(s);
        
        return answer;
    }
};

------------------------------------------------

### 문제 설명
정수 n을 입력받아 n의 약수를 모두 더한 값을 리턴하는 함수, solution을 완성해주세요.

제한 사항
n은 0 이상 3000이하인 정수입니다.

입출력 예
| n |	return |
|---|---|
| 12 |	28 |
| 5 |	6 | 

###### 입출력 예 설명
###### 입출력 예 #1
12의 약수는 1, 2, 3, 4, 6, 12입니다. 이를 모두 더하면 28입니다.

입출력 예 #2
5의 약수는 1, 5입니다. 이를 모두 더하면 6입니다.


#### Solution.java
------------------------------------------------
class Solution {
    public int solution(int n) {
    
        int answer = 0;
        
        for (int i = 0; i < n; i++) {
            if (n % i == 0) answer += i;
        }
        
        return answer;
    }
};

------------------------------------------------
