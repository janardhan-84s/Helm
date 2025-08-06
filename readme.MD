## HELM ##

Generally, we are having open source Images like Redis, RabbitMQ. We are not pushing the
images in Docker hub. 
similraly, like open source images.
we are having open source manifest files to run the images. we don't need to write manifest
files.using HELM we can achieve this.

## Advantages of Helm ##

1. using Helm we can install applications in k8, It is like a package manager in k8.
2. Templatise k8 manifest files

## Installing Helm ##

1. curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/main/scripts/  get-helm-3
2. chmod 700 get_helm.sh
3. ./get_helm.sh

## How to use Helm ##

1. The file must be "chart.yaml"
we place all our Hewlm information in "chart.yaml"

2. We can also creating a template folder to our main code
3. without touching the main code, if any changes are done in future and we need to update 
   them.
   We use "values.yaml " file 
4. In this values.yaml file we can write a section to our changes
5. In the main code we can refer to values.yaml file like this "{{ .Values.service.targetPort }}"