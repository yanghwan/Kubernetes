# Kubernetes
Kubernetes는 기본적으로 Google Kubernetes Engine (GKE)의 Runtime를 기본적으로 사용을 하였다.
이후 CRI(Container Runtime Interface) 및 CNI 등과 같이 기본기능들이 표준으로 자리를 잡으면서 다양한 런타임을 지원하게 되었다.
다양한 오케스트레이션 플램폼을 구축하기 위해서 런타임을 사용하기때문에  CRI(Container Runtime Interface) 기술은 표준으로 자리잡게 되었습니다.
최근 K8SS가 업계표준으로 자리잡고 점유하면서 Docker에서 무료 사용에 대한 이슈를 제기되면서 구굴에서는 CRI-O를 개발하게 되었으며, 서서히 CRI-O로 전환이 되고 있다.

 
- k8s별 cro 버전

|Version|Branch	Kubernetes branch/version|
|------|---|
|CRI-O 1.17.x |release-1.17	Kubernetes 1.17 branch, v1.17.x	|
|CRI-O 1.18.x |release-1.18	Kubernetes 1.18 branch, v1.18.x	|
|CRI-O 1.19.x |release-1.19	Kubernetes 1.19 branch, v1.19.x	|
|CRI-O HEAD   |master	Kubernetes master branch	?           |



- docker  
- Docker는 너무 무겁다. 

- DockerEE는 subscription 구매를 해야 한다.

- Docker Runtime의 불필요한 기능이 포함된 무거운 모듈

- 버그 픽스의 시간 소요 (Kubernetes에서 버그 픽스를 해야 함)

 

3) CRI-O는 무엇인가요?

- Docker -> CRI-O(Runtime), Podman(API)

- CRI-O는 구글에서 최초 개발

- PodMan은 Docker처럼 클러스터로 관리할 수 있음

- CRI-O는 Single node관리

- CRI-O는 Kubernetes를 위해 개발됨 (Only Kubernetes)

 

4) OCI 구성요소

- CRI-O (Runtime)

- PODMAN (API)

- BuildAH (이미지 빌드)

- Skepo (이미지 서버)



