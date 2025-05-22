This is a sample python app

Below things are covered in this project
1. Creating sample python app
2. Dockerize the app
3. Creating a helm chart
4. Push the docker image to docker.io
5. Deploying the helm chart to k3s cluster


Supporting commands - 
docker images
docker run -d -t -p 8280:8280 my-python-app
docker build -t my-python-app .
docker tag <src-image> <docker-hub-username>/<docker-image>:<version>
docker login -u <username> -p <password> docker.io
docker push <new-tagged-image>
helm install aditya-chart/ --generate-name