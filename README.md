## docker-cpp-hello-world
 Dockerize a cpp file with small image
 
 This repo builds an image which runs a cpp file <hello.cpp>, to do that we do the follwoing:
 
 # Create a cpp file <hello.cpp>
 
 # Create Dockerfile
 
 # Build the image
 docker build -t cpp-app .
 
 # Tag the image 
 docker tag cpp-app hazemelbaz/cpp-app:1.0
 
 # Run the container from inamge
 docker run -it --rm --name myapp cpp-app
 
 # Push the image to hub.docker
 docker push hazemelbaz/cpp-app:1.0
 
