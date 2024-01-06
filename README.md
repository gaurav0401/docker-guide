<h1>Docker Guide</h1>
<br>
<big>Docker is an open platform which packages application and its dependencies in a form of container.It used to developing , shipping and running an application.</big>

<h3> Docker Terminology </h3>
<ul>
    <li> <b> Docker File:</b> It is a text document which contains all those commands that will be used to assemble an docker image </li>
    <li><b>Docker Image:</b>It is a  template for creating a docker container.</li>
    <li><b>Docker Container:</b>It is the running instance of docker image.It holds entire package  to run application.</li>

                     build                        run
     Docker File -------------> Docker Image --------------> Docker Container 
</ul>

<br>
<br>
<h3>Installing Docker </h3>

<ul>
    <li>Install linux distro on your system  using <a href="https://youtu.be/eId6K8d0v6o?si=xdaBT47iu2rQYK4d">How to install wsl for windows 11.</a></li>
    <li>Now , go to the   <a href="https://docs.docker.com/engine/install/">Docker Engine  Install</a> and download docker according  of your operating system. </li>
    <li>Install  downloaded file of docker and restart you system. Then sign-up on docker.</li>
    <li>Now go to the cmd and type <big><b>'docker -v'</b></big> to check the version of the installed docker.</li>
    <li>Now run a given command to to run first docker image  <b>'docker run hello-world'</b>  , if the command get executed successfully it means docker has been successfully installed on your system.</li>
</ul>



<h3>Useful docker commands</h3>
<ul><li><b>code .:</b>used to open folder in a vs code</li>
    <li><b>docker -v:</b>used to check docker version.</li>
    <li><b>docker pull 'image name':</b>used to pull image from a repository.</li>
    <li><b>docker pull 'image name:tag name':</b>used to pull image  of specific version.</li>
    <li><b>docker images:</b> It lists all the available  images in our docker. </li>
    <li><b>docker search 'term':</b>used to search images related to particular name/term .</li>
    <li><b>docker run  'image name':</b>used to start container.</li>
    <li><b>docker ps:</b>It is used to shows the running containers.</li>
    <li><b>docker ps -a/--all:</b>It is used to show all containers.</li>
    <li><b>docker ps -n/-last:</b>It shows last created containers including all states.</li>
    <li><b>docker ps -f "status=running/exited":</b>It is used to show the filtered containers list based on thier status.</li>
    <li><b>docker run --name 'give name' -d 'image name /id':</b>It is used to provide a name to  container before running that  container   </li>
    <li><b>docker run --name 'give name' -it  -d 'image name':</b>Used to run image with interaction mode.</li>
    <li><b>docker exec -it 'container id' 'command':</b>It is used to run a new command for a running container.</li>
    <li><b>docker inspect 'container id':</b>used to inspect container.</li>
    <li><b>docker stop 'container name':</b>It is used to stop running container.</li>
    <li><b>docker stop 'container ids...':</b>used to stop multiple containers at once. </li>
    <li><b>docker rm 'container ids/name....':</b>used to remove containers.</li>
    <li><b>docker image rm 'image name':</b>Used to remove images.</li>
    <li><b>docker restart 'container name/id':</b>used to restart container again.</li>
    <li><b>docker login:</b>used to login into docker hub to our  push images there</li>
    <li><b>docker commit:</b>It is used to save a state of existing container as a new image.</li>
    <li><b>docker push :</b>used to push / upload docker images to docker hub.</li>
    <li><b>docker copy:</b>used to copy local files into docker image.</li>
    <li><b>docker logs:</b>used to retrieves logs of container at the time of execution.</li>
    <li><b>docker volume:</b>It is used to create  volumes to store data.</li>
    <li><b>docker log out:</b>used to log out from docker hub.</li>
    <li><b>WORKDIR: </b>used to set current  working directory for instructions in dockerfile.</li>
    <li><b>COPY: </b>used to copy files from source to destination directory.</li>
    <li><b>docker image rm $(docker image ls -a) </b>used to remove all images at once </li>
    <li><b>docker build -t 'image name' 'path(where docker file is located)':</b>used to create new image.</li>
    <li><b>docker run -p using port : allocated port (8001:8000) 'image name':</b>used to run container on a specific port number.</li>

</ul>



<h3>Building an image in docker</h3>
<ul>
    <li><b>Create dockerfile in the separate folder  with name 'Dockerfile' (Note:Dockerfile is no extension).</b></li>
    <li><b>Now write commands in docker files .</b></li>
    <li><b>Now go to terminal and write build command for creating an image from dockerfile which is mentioned above. </b></li>
    <li><b>It will takes sometime to create image. Once completed you can check your image using 'docker images' command. </b></li>
    <li><b>Now you can use that image to create containers.</b></li>
</ul>