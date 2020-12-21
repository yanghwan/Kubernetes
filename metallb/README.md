목적 : metallb 설치
생성 순서: metallb.yaml 설치 ex) kubectl apply -f metallb.yaml
비고 :
metallb-system 네임스페이스 사용
controller-xxxxxxxxxx-xxxxx (1개의 pod)
speaker-xxxxx (모든 노드에 pod)

Step 2. metallb 대역 설정
목적 : metallb에서 사용할 대역 설정 (호스트와 동일한 대역 사용)
생성 순서: metallb_cidr.yaml 적용 ex) kubectl apply -f metallb_cidr.yaml
비고 :
apiVersion: v1
kind: ConfigMap
metadata:
  namespace: metallb-system
  name: config
data:
  config: |
    address-pools:
    - name: default
      protocol: layer2
      addresses:
      - 172.22.8.160-172.22.8.180
      
