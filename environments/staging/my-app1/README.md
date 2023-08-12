# argocd
Notes:

Crated one nginx image form nginx
docker login --username user    #enter password

docker pull nginx:latest
docker tag nginx:latest dockerhunuser/nginx:latest
docker push dockerhunuser/nginx:latest

create Folder:


How to do port forwarding for service:

kubectl port-forward **-n namespace_name** **my-service** 8000:8080

here: 8080 service port and 8000 local port on which service can expose outside cluster

Exp: 
  - port: 8082
    targetPort: 80
    nodePort: 30008

service: **my-app2**

kubectl port-forward -n foo service/nginx 8082:8082

service: **my-app1**

kubectl port-forward -n bar service/guestbook 8081:8081
