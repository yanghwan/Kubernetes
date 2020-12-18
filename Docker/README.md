# Docker Runtime
Docker는 Contaienr가상화를 위한 런타임이며, Windows 및 Linux 환경에서 간단히 다운받아서 설치 및 활용할수 있습니다.
K8s 런타임 환경으로 이용 , Container 이미지를 만들기 위한 환경으로 이용 , 생성된 이미지를 테스트, Docker Registry 저장소  활용할수 있습니다.  

## 사용방법
### Docker Start 및 Stop
sudo service docker stop\
sudo systemctl daemon-reload\
sudo service docker start	\

### Docker 저장소 변경
Docker Runtime 위치는 OS 및 버전마다 다르기 때문에 해당파일를 수정하여 변경을 할수가 있습니다.\
graph는 특정버전이후 depreciated 되어 있기 때문에  data-root를 사용하기를 권장합니다.

|/etc/docker/daemon.json|
|---|
|{<br />"graph": "/storage/repository/docker" <br />}|
|{<br />"data-root": "/storage/repository/docker" <br />}|
