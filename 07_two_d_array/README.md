## 2차원 배열
* 배열 안에 배열이 자리 잡은 형태로 **2차원 배열** 이라고 한다. 
* 2차원 배열은 여러개의 1차원 배열을 가진 배열이다. 
* 첫 번째 범위는 저장 할 1차원 배열의 개수를 의미한다
* 두 번째 범위는 저장 한 1차원배열의 크기를 의미한다. 
* 1차원 배열의 크기는 모두 동일해야 한다. 

## 2차원 배열 초기화
```
int[][] scores = {
    {89, 93, 91, 93, 92, 78, 90, 90, 93, 90},
    {91, 82, 72, 98, 92, 87, 77, 87, 74, 88},
    {98, 93, 94, 91, 97, 94, 91, 96, 98, 90},
    {65, 63, 57, 87, 88, 92, 78, 85, 70, 68},
    {45, 50, 48, 63, 67, 58, 40, 66, 47, 64}
};
```

## 반복문을 통한 2차원 배열 접근
* 2차원 배열이므로 중첩 반복문이 효율적이다.

```
for (int i = 0; i < scores.length; i++) {  // 배열의 개수 만큼 반복(행)
    int sum = 0;
    for (int j = 0; j < scores[i].length; j++) {  // 1차원 배열 내의 개수 만큼 반복(열)
        sum += scores[i][j];
    }
    
    System.out.println("평균 점수는 " + sum / 10.0);
}
```

## 예제
### [예제 1](two_d_array_ex/Ex01.java) : 2차원 배열

## 문제
### [문제 1](two_d_array_quiz/quiz01/README.md) : 2차원 배열 입력
### [문제 2](two_d_array_quiz/quiz02/README.md) : 2차원 배열 다루기