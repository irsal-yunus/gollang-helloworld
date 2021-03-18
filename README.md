# create dockerfile golang apps
touch Dockerfile
git add .
git commit -m "add Dockerfile"
git push

# setting account connect automation build in docker hub

# pull image after build success in docker hub

docker pull ichalapyel/golang-helloworld:1.0