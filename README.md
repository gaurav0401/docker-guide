<h1>Docker Guide</h1>
<br>
<big>Docker is an open platform which packages application and its dependencies in a form of container.It used to developing , shipping and running an application.</big>

<h3>Terminology of Docker</h3>
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
    <li>Install linux distro on your system using wsl (windows subsystem for linux) using <a href="https://youtu.be/eId6K8d0v6o?si=xdaBT47iu2rQYK4d">How to install wsl for windows 11</a></li>
    <li>Now , go to the   <a href="https://docs.docker.com/engine/install/">Docker Engine  Install</a> and download docker according  of your operating system. </li>
    <li>Install  downloaded file of docker and restart you system. Then sign-up on docker.</li>
    <li>Now go to the cmd and type <big><b>'docker -v</b></big> to check the version of the installed docker.</li>
    <li>Now run a given command to to run first docker image  'docker run hello-world' , if the command get executed successfully it means docker has been successfully installed on your system.</li>
</ul>