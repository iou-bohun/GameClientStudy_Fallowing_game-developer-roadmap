# GameClientStudy_Fallowing_game-developer-roadmap
game-developer-roadmap https://github.com/utilForever/game-developer-roadmap 을 따라 학습하는 GameClient
- [Game_Mathematics](#Game_Mathematics)
  * [vector](#vector)
  * [Matrix](#Matrix)
  * [LinearAlgebra](#LinearAlgebra)
  * [Geometry](#Geometry)
  * [Affine_Space](#Affine_Space)
  * [Eular_Angle](#Eular_Angle)
  * [Quaternion](#Quaternion)
  * [Projection](#Projection)
  
- [Game_Pysics_#1](#Game_Pysics_#1)
- [Game_Engine](#Game_Engine)
- [Game_Physics_#2](#Game_Pysics_#2)
- [Computer_Graphics_#1](#Computer_Graphics_#1)
- [Graphics_API](#Graphics_API)
- [Computer_Graphics_#2](#Computer_Graphics_#2)
- [Game_AI_#1](#Game_AI_#1)
- [Game_AI_#2](#Game_AI_#2)
- [Advanced_Randering_#1](#Advanced_Randering_#1)
- [Advanced_Randering_#2](#Advanced_Randering_#2)
# Game_Mathematics 
### vector  
#### 백터의 내적 **(Vector3.Dot(Vertor a, Vector b))**

 - 내적을 이용해 두 백터간의 방향관계를 알 수 있다.

   ex)플레이어의 방향백터와 적으로의 방향백터가 음일 경우 적은 플레이어의 뒤에 있다 는 의미이다.

 - 내적을 이용해 어떤 백터를 중심으로 정해진 각범위 내에 물체가 존재하는지 판별하는데 유용하다.

   ex)적의 시야각=a, 적의 방향백터 = v, 적이 플레이어를 향하는 백터 = v 인 경우

   v,w사이의 각=b 가 a/2 보다 작다면 시야 범위에 있는것이다.

<img width="408" alt="image" src="https://user-images.githubusercontent.com/56661597/233840669-0f283dd4-db3c-47d1-8fe9-19fe7e9378ba.png">

   Cos(b)>Cos(a/2)인 경우

 #### 백터의 외적 **(Vector3.Cross(VectorA, VectorB))**

 - 두 벡터의 평행 여부를 판단할 때 사용한다. 
  
   외적을 했을 때 0이라면 평행이다.
  
 - 적이 플레이어의 오른쪽에 있는지, 왼쪽에 있는지 알 수 있다. 

   게임 속의 상향 벡터를 up, 플레이어의 전방 벡터를 v, 플레이어에서 적을 향하는 벡터를 w 라 할때
  
   up⋅(VxW)>0이면 적은 주인공의 오른쪽에 있는것이다. 
  
### Matrix

![image](https://user-images.githubusercontent.com/56661597/234601321-2a54baef-b1fc-4d5c-9d13-cfa959df3766.png)

 - 행렬은 row, column으로 이루져있고, 가로 세로로 나누어져있다.

   행렬이라는 하나의 묶음을 만들어 계산을 한번에 하게 한다
  
   게임의 행렬은 위치,크기,회전을 행렬로 처리한다. (Transform)
   
   행렬을 통해 하나의 조합을 만들고 reusable하게 만들어 연산량을 줄이는게 목적이다. 

### LinearAlgebra

 - 벡터공간, 벡터, 선형변환, 행렬, 연립 선형 방정식 등을 연구하는 대수학의 한 분야. 

   벡터 공간이란 = 선형결합 연산이 같은 공간산에 존재하는 벡터들이 모인 공간. 
   
### Geometry
 
 - 도형을 연구하는 수학. ex) 피타고라스 정리 
 
   collision의 충돌 감지에 사용되었다. 
   
 ### Affine_Space
 
 - 벡터는 크기와 방향만 가지므로 정적인 위치를 표현하기에는 무리가 있다. 
   이를 해결하기 위해 point 를 사용한다. 이러한 점을 찍을수 있는 공간을 아핀 공간이라고 한다. 
    
   polygon과 관련이 있다.

 ### Eular_Angle
 
 - x,y,z, 3개 축을 기준으로 회전시키는 우리가 흔히 알고있는 각도계 

   x > y > z 순으로 오일러 앵글이 계산된다. 

   짐벌락 문제가 생긴다. 짐벌락 = 같은방향으로 오브젝트의 두 회전 축이 겹치는 현상. 
   
   https://www.youtube.com/watch?v=zc8b2Jo7mno&feature=youtu.be&t=2m9s

 ### Quaternion 
 
-  **Quaternion.Eular**
 
   각 축을 한번에 계산/ 4개의 성분 x,y,z,w 로 이루어져 있다. w는 스칼라 
 
   물체의 회전에 사용된다. transform.rotation = Quarternion.Eular(new Vector3(x,y,z))
   
 ### Projection
 - Parallel Projection / Orthographic projection
   
   원근감이 없는 투영. 물체들의 절대적인 크기를 봐야 할 때 사용된다.
   
 - Perspective Projection

   원근감이 있는 투영.\ㅑㅕ숔로ㅛㅑㅐㅔ 
   
# Game_Pysics_#1
# Game_Engine
# Game_Physics_#2
# Computer_Graphics_#1
# Graphics_API
# Computer_Graphics_#2
# Game_AI_#1
# Game_AI_#2
# Advanced_Randering_#1
# Advanced_Randering_#2
