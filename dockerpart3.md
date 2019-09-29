#services

creat docker-compose.yml 
listed in the docekrcontainer

    docekr-machine ls 

![machine ls](/images/machine-ls.PNG)


add nodes

    docker-machine ssh myvm1 "docker swarm init --advertise-addr <myvm1 ip>"


![myvm1](/images/jionmyvm1.PNG)


add worker
    
     docker-machine ssh myvm2 "docker swarm join \
    --token <token> \
    <ip>:2377"
![myvm2](/images/jionmyvm2.PNG)

deploy

    docker stack deploy -c docker-compose.yml getstartedlab
![deploy](/images/stack.PNG)

    docker stack ps getstartedlab
![stack ps](/images/psstack.PNG)    
    

