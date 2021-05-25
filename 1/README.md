
# 가희와 함께 하는 코딩 테스트 1회
5월 23일 13시부터 18시까지 1회 코딩테스트가 열렸습니다.   
1회 코딩 테스트에서 보고자 했던 것은 **조건을 얼마나 잘 읽느냐**였습니다.  
어떤 것을 읽어내는 것이 중요했는지 1, 4, 5번 문제를 브리핑 해 보겠습니다.

## 21771. 가희야 거기서 자는 거 아니야
[바로 가기](https://www.acmicpc.net/problem/21771)  

* **베개 중의 일부가 가희에 의해서 가려진 상태**라면, 가희는 베게 위에서 자고 있습니다.  
* 가희는 베개 위에서 자고 있거나, 베개 아래에서 자고 있습니다.  

즉, 가희의 일부도 가려지고, 베개의 일부도 가려지는 경우는 없음을 알 수 있습니다. 따라서,  _P_ 와 _G_ 가 몇 번 나오는지만 보면 됩니다.  

## 21774. 가희와 로그 파일
[바로 가기](https://www.acmicpc.net/problem/21774)  

시간 제한을 보면 2초로 꽤 넉넉함을 알 수 있습니다. 시각 데이터는 60만개 주어집니다.  
문자열의 길이는 최대 20자이고, 60만개의 시각이 들어올 때, 1200만 x 20 = 2.4억이 됩니다.  
이 부분은 구분자를 가지고 _long long_ 형으로 압축한다면, 20이 빠질 수 있습니다.  
  
이 문제에서 더 중요했던 점은 아래 2가지 입니다.  
* 주어진 시작 시각과 종료 시각 **사이**에, ~
* 시각은 **YYYY-MM-DD hh:mm:ss형식**으로 주어진다.
  
형식이 같고 시각의 선후 관계만 파악하면 되므로, 문자열로 처리하면 됩니다.

## 21775. 가희의 자원놀이
[바로 가기](https://www.acmicpc.net/problem/21775)  

문제가 상당히 긴 편이여서, 조건을 잡기가 쉽지 않았습니다.  
체감 난이도를 결정지었던 결정적인 조건은 아래와 같습니다.
 
* 자원 카드  _n_ 을 획득한 사람이 다시 _acquire  n_ 을 수행하지 않는다.
* 획득하지 않은 자원 카드를 시각은 _release_ 하는 경우는 없다.
  
그렇기 때문에, **자원을 누군가 가지고 있는지**만 관리하면 됩니다.