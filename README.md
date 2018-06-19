# kubernetes_training
Training stuff
```
•	Demonized containers : run in background
•	Interactive containers: 
•	Ctl +pq –for disconnecting to a running container without killing the docker.
•	Dhclient ---for getting ip when interphase was connected in host mode. 
•	https://github.com/amitvashist7/kubernetes-project/tree/master/setup training stuff
•	download https://storage.googleapis.com/minikube/releases/latest/minikube-windows-amd64.exe or minikube for Windows and install from command line….rename minikube.exe.
•	.\minikube.exe start --- will download the image on windows.
•	https://kubernetes.io/docs/tasks/tools/install-kubectl/#install-with-chocolatey-on-windows
Above link has Windows curl to download kubectl for windows. (curl -LO https://storage.googleapis.com/kubernetes-release/release/v1.10.3/bin/windows/amd64/kubectl.exe)

•	Vagrant init ---with vagrant file in current locatin.
•	Vagrant status
•	Vagrant ssh kuber-master
•	Echo ‘export $KUBECONFIG=/etc/kubernetes/admin.conf’ >> ~/.bash.rc
•	Kubectl create –f <file/dir>
•	Kubectl get pods –o wide
•	Kubectl describe pod <pod name>
•	Kubectl delete pod <pod>
•	Kubectl delete service <pod>
•	Kubectl get rc
•	Kubectl edit rc hellowordo-controller
•	Kubectl scale –replicas=1 rc helloworld-controller
•	Kubectl delete rc helloworld-controller
•	Git repo got to deployment
•	Kubectl create –f helloworld.yml
•	Kubectl get deployments
•	Kubectl get pods
•	Kubectl get pods –show-labels
•	Kubectl rollout status deployments/helloworld-deployments
•	Kubectl expose deployment hellowrodl-deployment –type=NodePort
•	Kubectl get services.
•	Kubectl describe service helloworld-deployment
•	Kubectl get deployment 
•	Kubectl set image deployment helloworld-deployment k8s-demo=amitvashist7/k8s-tiny-web:2
•	Kubectl rollout status deployment helloworld-deployment
•	Kubectl rollout undo deployment helloworld-deployment
•	Kubectl set image deployment helloworld-deployment k8s-demo=amitvashist7/k8s-tiny-web:1
•	Kubectl rollout history deployment helloworld-deployment deployments “helloworold-deployment”
•	Kubectl rollout history deployment helloworld-deployment –revision=1
•	Kubectl rollout undo deployment helloworld-deployment –to-revision=1
			Service :
•	Kubectl expose –nodeport/clusterip/load balance.
•	Ingress traffic will come in if we use load balance.
•	DNS name can be used using service discovery. 
•	Port range 30000-320767 –random port.
•	Kubectl create –f helloworld.yml
•	Kubectl create –f helloworld-nodeport-service.yml
•	Kubectl describe services helloworld-service
•	Kubectl expose pod helloworld
•	Kubectl expose pod helloworld –type=NodePort

Labels
o	Labe can be applied to pods/nodes (nodeSelector).
o	Kubectl get nodes –show-labels
o	Kubectl label node worker01 hardware=high
o	Kubectl label node worker02 hardware=low
o	Kubectl get nodes –show-labels
o	kubectl create –f hellowrod-nodeselector.yml
o	kubectl get deployments

		Health check
o	URL Health check
o	Command status check
o	Kubectl create –f helloworld-healthcheck.yml.
o	Kubectl logs <node>/<pod>
o	Kubectl get events
		Secrets 
o	Username/passwd/keys/secret data etc.
o	Environment variable.
o	Stores in file
o	.env file to store secrets
o	Echo –n > “root” ./username.txt
o	Echo –n>”passwd” ./password.txt
o	Kubectl create secret generic db-user-pass –from-file=./username.txt –from-file=./password.txt
o	Echo –n “root”|base64 ---create hashes 

```
