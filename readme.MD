## HELM ##

Generally, we are having poen source Imgaesw like Redis, RabbitMQ. We are not pushing the
images in Docker hub. 
similraly, like open source images.
we are having open source manifest files to run the images. we don't need to write manifest
files.using HELM we can achieve this.

## Advantages of Helm ##

1. using Helm we can install applications in k8, It is like a package manager in k8.
2. Templatise k8 manifest files

## Installing Helm ##

curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3
chmod 700 get_helm.sh
./get_helm.sh

## How to use Helm ##

The file must be "chart.yaml"
we place all our Hewlm information in "chart.yaml"