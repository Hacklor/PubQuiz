# Concourse-Build-Docker-Image



---getting up Concourse.ci ---

install docker

then download docker-compose file to get concourse nodes up and running

wget https://concourse-ci.org/docker-compose.yml

docker-compose up -d

now hit the http://localhost:8080 in your browser

check Concourse ci is up

now install fly as per your system available on ui

--- fly setup ---

login and get authenticated with fly

fly -t main -c http://localhost:8080
click on the given link for token authenticaation

now all set up

---git setup---

Fork the https://github.com/Hacklor/PubQuiz

clone it to your local dir

cd PubQuiz

mkdir Concourse

create these two file ( available at https://github.com/dharmendrakariya/PubQuiz/blob/master/Concourse/ ) 
nano pipeline.yml
nano Dockerfile

now git add, commit and push all the changes to github 

--- creating the pipeline with the help of pipeline.yml ---

set_pipeline having name my_pipeline

fly -t main set-pipeline -p my_pipeline -c pipeline.yml

unpause it

fly -t main unpause-pipeline -p my_pipeline

hit the localhost:8080 and publish the pipeline

after successful run, check the dockerhub account and the newly added dockerimage.
