


kubeadm config print init-defaults  #init시 기본값들을 출력해준다.
                                                                                      
[root@y-master01 hypercloud-install-guide]# kubeadm config print init-defaults
--> kubeadm 실행시 기본적인 환경정보를 확인할수 있습니다. (Runtime)

- k8s에 조인이 되지 않거나 Key를 저장하지 않는경우에는  master node에서 아래 명령어를 통해 token 재생성이 가능하다.\
 kubeadm token create --print-join-command \
 
\# kubeadm token create --print-join-command \
W1221 21:29:03.795887    1917 validation.go:28] Cannot validate kube-proxy config - no validator is available \
W1221 21:29:03.795960    1917 validation.go:28] Cannot validate kubelet config - no validator is available \
kubeadm join 10.17.33.83:6443 --token bixz2y.xlxnt3ua5ims7oh1     --discovery-token-ca-cert-hash sha256:632a700b246a923fdd4481906236f5c8db4d70bffcd8297e2e6c47524cd39e05  \ 

 
