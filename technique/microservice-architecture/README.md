# 출제 의도
1. 최신 기술에 대해서 관심이 있는가?
## 문제
Q1. Microservice Architecture 를 알고 계시다면, 알고 있는대로 설명해주세요.
<details><summary>Q1. 답</summary>
<pre>
빠르게 확장되고 있는 현재의 시스템들을 위한 아키텍처라고 할 수 있습니다.

기존의 Monolith 방식과는 다르게 구성하기 나름이지만 조각으로 나눠서 기능별로 Monolith 를 구성하는 방식입니다.
해당 방식을 구현하게 되면 서로 상호작용 하기 때문에 에러가 나면 디버깅을 하기 힘들 수 있다는 단점이 있지만 설계를 제대로 하면, 극복이 가능합니다.
단점이 곧 장점이 될 수 있습니다.
상호작용을 하지 않는 기능들이라면, A service 가 down 되도 B service 에는 영향이 있지 않을 것 입니다.

대표적인 장점이 확장하기가 쉽습니다.
A 라는 서비스에 유저가 몰렸다면, A monolith 환경인 패키지를 여러 개를 작동 시키면 됩니다.
그리고 위의 layer 에서 추가된 환경에 대해서 설정을 추가하면 간단하게 많은 유저를 활동시킬 수 있는거죠.

단점은 많지 않은 유저를 위해서 서버를 엄청 많이 띄워놔야 된다는 것 입니다.
곧 비용으로 연결되니 손해가 클 것 같습니다.


정리하면
--- 단점 ---
1. 너무 작은 단위로 구성하면 필요없는 비용이 나감
2. 설계를 잘못하게 되면 chaos 현상이 나타남 (에러)
3. 관리할 수 있는 인력이 많지 않음
--- 장점 ---
1. 빠른 확장성
2. 비용 절감이 가능할 수 있음
3. 여러 가지의 언어로 각각의 맞는 서비스를 구성 가능함
4. 각각의 서비스 별로 팀을 구성해서 책임감이 커질 가능성이 있습니다. -> 품질 향상

이외에도 많지만 생각이 안남
</pre>
</details>