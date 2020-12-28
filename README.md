# ft_services_materials

docker <br />
docker commands:<br />
docker pull xxx <br />
docker run -d -p 8080:80 -p 3000:80 xxx <br />
docker ps <br />
docker start xxx <br />
docker stop (id/name) <br />
docker image ls <br />
docker ps -a <br />
docker rmi (id) ;rm image <br />
docker rm (id) <br />
docker rm $(docker ps -aq) ;rm all stopped container  <br />
docker run --name xxx <br />
docker -v $(pwd):/usr/share/nginx/html:ro ;store static files, delete :ro, then new files can be created <br />
docker exec -it (name) bash ;go into the container system <br />

Using dockefile <br />
docker build -t xxx . <br />
docker tag xxx(old) xxx(new) <br />

docker debug: <br />
docker inspect (id/name) <br />
docker -f logs (id) ; -f, shows the logs at real time<br />

https://www.youtube.com/watch?v=Wf2eSG3owoA&feature=youtu.be<br />

nginx<br />
https://www.it-connect.fr/configurer-nginx-en-tant-que-reverse-proxy/ <br />
https://linuxize.com/post/nginx-reverse-proxy/ <br />
https://dev.to/danielkun/nginx-everything-about-proxypass-2ona <br />

kubernetes <br />
kubernetes commands: <br />
minikube version <br />
minikube start <br />
minikube service (name) ;assign  external IP<br /> 
kubectl version <br />
kubectl cluster-info <br />
kubectl get nodes <br />

kubectl create deployment hello-node --image=k8s.gcr.io/echoserver:1.4 ; Use the kubectl create command to create a Deployment that manages a Pod. The Pod runs a Container based on the provided Docker image. <br />
kubectl get deployments <br />
kubectl get pods <br />
kubectl get events <br />
kubectl config view <br />
kubectl expose deployment hello-node --type=LoadBalancer --port=8080 ; To make the hello-node Container accessible from outside the Kubernetes virtual network, you have to expose the Pod as a Kubernetes Service. <br />
kubectl get services <br />
kubectl delete service hello-node <br />
kubectl delete deployment hello-node <br />
minikube stop <br />
minikube delete <br />

kubectl get - list resources <br />
kubectl describe - show detailed information about a resource <br />
kubectl logs - print the logs from a container in a pod <br />
kubectl exec - execute a command on a container in a pod <br />
kubectl exec deploy/DEPLOYMENT -- pkill APP <br />

metallb: <br />
https://www.youtube.com/watch?v=xYiYIjlAgHY<br />

ftps: <br />
https://security.appspot.com/vsftpd/vsftpd_conf.html vsftpd<br />
https://www.jscape.com/blog/bid/80512/active-v-s-passive-ftp-simplified <br /> 
https://www.pixelstech.net/article/1364817664-FTP-active-mode-and-passive-mode<br />
https://www.digitalocean.com/community/tutorials/how-to-set-up-vsftpd-for-a-user-s-directory-on-debian-10 <br />
https://superuser.com/questions/265062/downloading-file-from-ftp-using-curl <br />
https://itgala.xyz/how-to-upload-a-file-to-remote-ftps-with-curl-and-php/ <br />
https://www.howtoforge.com/tutorial/how-to-use-ftp-on-the-linux-shell/ <br />

grafana: <br />
https://www.datadoghq.com/blog/how-to-collect-and-graph-kubernetes-metrics/ <br />
https://grafana.com/docs/grafana/latest/administration/provisioning/#datasources <br />

wordpress: <br />
https://codingwithmanny.medium.com/custom-wordpress-docker-setup-8851e98e6b8<br />

sshcommand <br />
ssh user@host -p port -vvv <br />



