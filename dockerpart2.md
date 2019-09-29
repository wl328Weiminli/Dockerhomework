# Docker container

prepare the file 

![prepare file](/images/prepare.PNG)

all of the file listed in the dockercontainer folder

build the friendlyhello

    docker build --tag=friendlyhello .

![build](/images/build.PNG)

Run the app

    docker run -p 4000:80 friendlyhello

![run app](/images/run.PNG)

![display](/images/display.PNG)

stop the container
    docker container ls
    docker container stop container id
![stop](/images/stop.PNG)

Tag the image

    docker tag friendlyhello wl328lwm/get-started:part2

![tag](/images/tagimage.PNG)

publish the image 
    docker push wl328lwm/get-started:part2

![publish](/images/dockerpush.PNG)
![dockerhub](/images/pushed.PNG)



