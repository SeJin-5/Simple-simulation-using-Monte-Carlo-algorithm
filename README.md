## 몬테카를로 알고리즘을 이용하여 원주율 계산하기

1. [1,0] X [0,1]에서 점 (x,y)를 표집한다.
2. 표집한 점의 중심이 (0,0)에 있고 반지름이 1인 원에 속하는지 계산한다. 이는 원의 정의에 따라 x<sup>2</sup>+y<sup>2</sup>과 1을 비교함으로써 계산할 수 있다.
3. 위의 두 과정을 충분히 반복하여, 원에 속한 점들의 개수를 계산한다. 표집 영역과 원의 공통 영역은 $\pi$/4 의 넓이를 가지며, 원에 속한 점의 개수를 전체 점 개수로 나눈 비율은 \pi/4 값에 근사하게 된다.

### 반복횟수 100
![반복횟수 100 이미지](https://i.esdrop.com/d/f/3X5MiUW5Gr/X8SUiltN0y.png)

### 반복횟수 10,000
![반복횟수 10,000 이미지](https://i.esdrop.com/d/t/3X5MiUW5Gr/iLHkx1xkvo.jpg)

### 반복횟수 100,000
![반복횟수 100,000 이미지](https://i.esdrop.com/d/t/3X5MiUW5Gr/5kUTtnvz94.jpg)

#### 프로젝트 수행 후기
 반복횟수가 많아질수록 실제 \pi 값인 3.14의 근사치로 다가간다. 난수 생성이 늘어날수록 우리가 원하는 정보 값이 근사치에 근접하는 몬테카를로 알고리즘의 특성을 보여준다.
