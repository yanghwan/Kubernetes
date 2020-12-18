
Docker Runtime을 이용하여 Image를 만들거나 Private Registry를 구축하여 이용할수 있습니다.


- Docker Start 및 Stop\
sudo service docker stop	
sudo systemctl daemon-reload
sudo service docker start	

Docker Runtime 위치는 OS 및 버전마다 다르기 때문에 해당파일를 수정하여 변경을 할수가 있습니다.\
graph는 특정버전이후 depreciated 되어 있기 때문에  data-root를 사용하기를 권장합니다.

- Docker Runtime 변경
|/etc/docker/daemon.json|
|---|
|{<br />"graph": "/storage/repository/docker" <br />}|
|{<br />"data-root": "/storage/repository/docker"<br />}|
