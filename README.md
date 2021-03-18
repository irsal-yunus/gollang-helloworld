# create dockerfile golang apps
touch Dockerfile

# build image golang-helloword
docker build -t golang-helloword:1.0 .

# run container image 
docker run -p 8000:8000 golang-helloworld
docker run -d -p 5000:5000 --name registry registry:2
# push image docker registry
# example using docker hub local

docker commit 354588d82cc6 gollang-helloworld:1.0
docker push golang-helloworld:1.0