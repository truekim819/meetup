# 스피드 짝코딩 규칙

- 팀 전체에서 코더 1명, 나머지는 주자로 1회씩 참여

- 문제를 고르고 순서를 정하면 전체 문제가 한번에 공개됨

- 전체 문제 공개와 함께 타이머 시작

- 코딩 중 결과 확인 허용

- 문제 패스 허용

- 코드가 완성되었다고 판단되면 주자를 바꾸고 다음 문제 진행

- 문제가 넘어가면 이전 문제 파일은 수정 불가능

- 주자나 코더 이외의 팀원은 주자나 코더에게 지시하면 탈락

- 모든 문제를 다 풀었으면 타이머 종료

- 승리 조건
	- 맞춘 문제 개수가 많을 수록 승리
	- 문제 개수가 같으면 시간이 더 빠른쪽이 승리

- 의미 없는 코드로 echo 연속 사용 및 echo로 문자열 만들면 탈락

	```
	(X)
	echo '*';
	echo '*';
	echo ' ';
	echo ' ';
	```

	```
	(X)
	echo '*';
	$n = 1;
	echo '*';
	```

	```
	(X)
	echo '**';
	echo '* * *';
	```

	```
	(O) 의미 있는 줄바꿈을 위한 연속 사용 허용
	echo "*\n";
	echo "*";
	echo "\n";
	```

- 단순한 코딩이 아닌 구현 자체를 설명하면 탈락

	- (X) 한줄마다 별을 1개씩 출력하는 for문을 만들어주세요.

	- (X) 조금전 문제랑 똑같은데 짝수대신 홀수로 할거거든요.

	- (O) $i가 0부터 10까지 1씩 증가하는 for문을 선언해주세요. for문안에 echo로 별과 \n을 출력해주세요.

- 함수 및 클래스 사용 불가

	- 허용 구문: if, switch, for, foreach, while

	- 출력 방법: echo

	- 데이터형: int, string, array
