# Music-Motion
## Speedy Music      
https://vimeo.com/845897735/1e6fa712c2?share=copy  
![demo-movie](https://github.com/melody-sigma/LOLMusiK/assets/36034521/fae80781-09dd-48af-a02b-942b04238d37)  

## 딥러닝에 때려박기(일반적으로 제일 처음 떠오르는 아이디어)   
  - 오버피팅, 언더피팅일때 음악의 특징을 직접 참조하여 외워버리는 특성이 존재  
  - 패턴이 이상하게 추출되거나 아예 감지조차 못함  
  - 완전히 새로운 분위기의 음원이 들어오면 사.실.상. 인간이 플레이할수 있게끔 패턴 만들어주는 방법 따윈 불ㅋ가ㅋ  

## 리듬액션 게임에서의 적용 문제점  
  - 전통적인 접근 방법은 
머신러닝이 아닌 음악 비트 특징을 감지하는 일반 규칙을 사용.  
  - 시간의 흐름에 따라 음악 비트, 클라이막스 의 통계적 분포가 수시로 바뀜.  
  - CNN-LSTM도 이론상 가능. 하지만, 보여준 샘플들 전체의 분포를 학습하지는 않음.  

## 해결하기 위한 시도  
  - 전체 분포를 아예 일반화하여 간접적으로 학습하는 모델이 필요  
  - 음원과 노트 시계열 특징을 배우고 이와 비슷하게 특징 벡터가 추출,  
오디오 입력이 들어오면 이를 기반으로 진짜 플레이 노트 패턴처럼 생성하는 모델이 필요  
  - 이처럼 생성 모델은 데이터 증강에도 써먹을수 있음  
  - 솔루션 : Time GAN
  - 
