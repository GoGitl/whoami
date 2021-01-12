whoami with arm support 
======
Raspberry / ARM support via specific cpu tag

Simple HTTP docker service that prints it's container ID

    $ docker run -d -p 8080:8080 --name whoami -t gogitl/whoami
    736ab83843bb12dddd8b09969433f3a02d64d5b0be48f7a5c59a594e3a6a3541
    
    $ curl $(hostname --all-ip-addresses | awk '{print $1}'):8080
    I'm 736ab83837bb

You can find me on docker hub: [gogitl/whoami on Docker](https://hub.docker.com/repository/docker/gogitl/whoami)