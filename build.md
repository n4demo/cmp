# CMP

## Create the CMP Docker image
docker image build . -t node4demo/cmp:latest -t node4demo/cmp:0.1.2 -t node4demo/n4stack-manage:0.1.2 -t node4demo/n4stack-manage:latest

## run it to test
docker container run --name cmp --rm -it node4demo/cmp:latest

## login to docker Hub
docker login --username node4demo -p my-password
docker push node4demo/cmp:latest
docker push node4demo/cmp:0.1.1
docker push node4demo/n4stack-manage:latest
docker push node4demo/n4stack-manage:0.1.2
docker stop xxx

## now run container locally
docker container run --name cmp --rm -it node4demo/cmp:latest

## run login command to login to Azure
bash5.1# ./login

bash5.1# cat sr
bash5.1# cat gp