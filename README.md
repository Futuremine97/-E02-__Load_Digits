# -E02-__Load_Digits
https://nvidiaupup.tistory.com/manage/newpost/26?type=post&returnURL=https%3A%2F%2Fnvidiaupup.tistory.com%2F26
암은 FN, 가짜 네거티브 가 적어야 합니다. 
이번에 저는 중대한 발견을 하였습니다<br>
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

