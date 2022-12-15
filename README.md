# cloud-project

first, clone the project.

then, create docker images from Dockerfiles:

docker build -t nginx-custom nginx/
docker build -t java-custom java-pingpong/
docker build -t nodejs-custom nodejs-pingpong/


then, run this commands to create 3 docker containers from this images:

docker run -dit --name nginx -p 8000:80 --network=new_bridge nginx-custom  
docker run -dit --name PingPong.java -p 8080:8080 --network=new_bridge java-custom  
docker run -dit --name PingPong.js -p 3001:3001 --network=new_bridge nodejs-custom


Now, open http://localhost:8000/ping in your browser.
