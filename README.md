# -E02-__Load_Digits
https://nvidiaupup.tistory.com/manage/newpost/26?type=post&returnURL=https%3A%2F%2Fnvidiaupup.tistory.com%2F26<br>

암 검진은 FN, 가짜 네거티브 가 적어야 합니다. <br>
그런데 다른 것들을 보니 예시 설명과는 다르게 2*2행렬이 아니라서 일일이 오류를 보기가 굉장히 어려워졌습니다<br>
그래서 유투브를 보니까 대각선 라인은 (n,n) 원소라서 맞는 경우의 수라는 것을 확인하였습니다 <br>

나머지는 오류라는 뜻이겠죠 <br>
정규롸를 시킨뒤, <br>
오류를 다 모아서 비교해보면 최고의 모델을 가려낼 수 있을 것 같습니다! (가정) <br>
 
그러다가 저는 중대한 발견을 하였습니다<br>
대각행렬를 다루는 것인데요 <br>
대각선에 있는 것들만 더해주려면 특별한 함수를 써야 합니다
<br>

print('-'*90)<br>

a2 = 0<br>

print('-'*90)<br>

for value1 in range(2,-2,-1):<br>

    d2 = np.diag(array1,k= value1)<br>

    a2 = a2 + np.sum(d2)<br>

print(a2)<br>


d29 = np.sum(np.diag(array1,k=0))<br>

print(a2-d29)<br>

e2 = a2 - d29<br>

print("제가 만든 성능지표는 : ")<br>

print(e2/a2)<br>

