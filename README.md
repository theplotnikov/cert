this repository has the Jenkinsfile that:
1. with terraform's create.tf will create two instances in yandexcloud.
2. with ansible's plabook.yml will tune these instances.
   first instance for building war project.
   second instance for deploying project with tomcat8.
   
before start this pipeline you must:
1. add credential in Jenkins. kind "ssh with private key", ID "privatekey", username "ubuntu", and content of yours privatekey.
2. prepare YC private data: cloud id, folder id, token, pubkey.
