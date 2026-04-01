# workstation-dev


## 터미널 컨트롤 로그
ryusungeun@SungEuns-MacBook-Pro Codyssey % git clone https://github.com/loader1017/workstation-dev.git
Cloning into 'workstation-dev'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.
ryusungeun@SungEuns-MacBook-Pro Codyssey % cd workstation-dev
ryusungeun@SungEuns-MacBook-Pro workstation-dev % pwd
/Users/ryusungeun/Desktop/2026/Codyssey/workstation-dev
ryusungeun@SungEuns-MacBook-Pro workstation-dev % ls -la
total 8
drwxr-xr-x   4 ryusungeun  staff  128 Apr  1 14:32 .
drwxr-xr-x@  4 ryusungeun  staff  128 Apr  1 14:32 ..
drwxr-xr-x  12 ryusungeun  staff  384 Apr  1 14:32 .git
-rw-r--r--   1 ryusungeun  staff   17 Apr  1 14:32 README.md
ryusungeun@SungEuns-MacBook-Pro workstation-dev % mkdir practice 
ryusungeun@SungEuns-MacBook-Pro workstation-dev % cd practice
ryusungeun@SungEuns-MacBook-Pro practice % touch test.txt
ryusungeun@SungEuns-MacBook-Pro practice % cat test.txt
ryusungeun@SungEuns-MacBook-Pro practice % cd ..
ryusungeun@SungEuns-MacBook-Pro workstation-dev % cd practice
ryusungeun@SungEuns-MacBook-Pro practice % cd .
ryusungeun@SungEuns-MacBook-Pro practice % cd ..
ryusungeun@SungEuns-MacBook-Pro workstation-dev % ls -ld practice practice/test.txt
drwxr-xr-x  3 ryusungeun  staff  96 Apr  1 14:33 practice
-rw-r--r--  1 ryusungeun  staff   0 Apr  1 14:33 practice/test.txt
ryusungeun@SungEuns-MacBook-Pro workstation-dev % chmod 755 practice/text.txt 
chmod: practice/text.txt: No such file or directory
ryusungeun@SungEuns-MacBook-Pro workstation-dev % chmod 755 practice/test.txt
ryusungeun@SungEuns-MacBook-Pro workstation-dev % chmod 700 practice
ryusungeun@SungEuns-MacBook-Pro workstation-dev % ls -ld practice practice/test.txt
drwx------  3 ryusungeun  staff  96 Apr  1 14:33 practice
-rwxr-xr-x  1 ryusungeun  staff   0 Apr  1 14:33 practice/test.txt
ryusungeun@SungEuns-MacBook-Pro workstation-dev % 

## Docker 컨트롤 로그
Last login: Wed Apr  1 14:38:46 on ttys000
ryusungeun@SungEuns-MacBook-Pro ~ % docker --version
Docker version 29.3.1, build c2be9cc
ryusungeun@SungEuns-MacBook-Pro ~ % docker info
Client:
 Version:    29.3.1
 Context:    desktop-linux
 Debug Mode: false
 Plugins:
  agent: Docker AI Agent Runner (Docker Inc.)
    Version:  v1.34.0
    Path:     /Users/ryusungeun/.docker/cli-plugins/docker-agent
  ai: Docker AI Agent - Ask Gordon (Docker Inc.)
    Version:  v1.20.1
    Path:     /Users/ryusungeun/.docker/cli-plugins/docker-ai
  buildx: Docker Buildx (Docker Inc.)
    Version:  v0.32.1-desktop.1
    Path:     /Users/ryusungeun/.docker/cli-plugins/docker-buildx
  compose: Docker Compose (Docker Inc.)
    Version:  v5.1.1
    Path:     /Users/ryusungeun/.docker/cli-plugins/docker-compose
  debug: Get a shell into any image or container (Docker Inc.)
    Version:  0.0.47
    Path:     /Users/ryusungeun/.docker/cli-plugins/docker-debug
  desktop: Docker Desktop commands (Docker Inc.)
    Version:  v0.3.0
    Path:     /Users/ryusungeun/.docker/cli-plugins/docker-desktop
  dhi: CLI for managing Docker Hardened Images (Docker Inc.)
    Version:  v0.0.2
    Path:     /Users/ryusungeun/.docker/cli-plugins/docker-dhi
  extension: Manages Docker extensions (Docker Inc.)
    Version:  v0.2.31
    Path:     /Users/ryusungeun/.docker/cli-plugins/docker-extension
  init: Creates Docker-related starter files for your project (Docker Inc.)
    Version:  v1.4.0
    Path:     /Users/ryusungeun/.docker/cli-plugins/docker-init
  mcp: Docker MCP Plugin (Docker Inc.)
    Version:  v0.40.3
    Path:     /Users/ryusungeun/.docker/cli-plugins/docker-mcp
  model: Docker Model Runner (Docker Inc.)
    Version:  v1.1.28
    Path:     /Users/ryusungeun/.docker/cli-plugins/docker-model
  offload: Docker Offload (Docker Inc.)
    Version:  v0.5.77
    Path:     /Users/ryusungeun/.docker/cli-plugins/docker-offload
  pass: Docker Pass Secrets Manager Plugin (beta) (Docker Inc.)
    Version:  v0.0.24
    Path:     /Users/ryusungeun/.docker/cli-plugins/docker-pass
  sandbox: Docker Sandbox (Docker Inc.)
    Version:  v0.12.0
    Path:     /Users/ryusungeun/.docker/cli-plugins/docker-sandbox
  sbom: View the packaged-based Software Bill Of Materials (SBOM) for an image (Anchore Inc.)
    Version:  0.6.0
    Path:     /Users/ryusungeun/.docker/cli-plugins/docker-sbom
  scout: Docker Scout (Docker Inc.)
    Version:  v1.20.3
    Path:     /Users/ryusungeun/.docker/cli-plugins/docker-scout

Server:
failed to connect to the docker API at unix:///Users/ryusungeun/.docker/run/docker.sock; check if the path is correct and if the daemon is running: dial unix /Users/ryusungeun/.docker/run/docker.sock: connect: no such file or directory
ryusungeun@SungEuns-MacBook-Pro ~ % docker ps
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
ryusungeun@SungEuns-MacBook-Pro ~ % docker run hello-world

Hello from Docker!
This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:
 1. The Docker client contacted the Docker daemon.
 2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
    (arm64v8)
 3. The Docker daemon created a new container from that image which runs the
    executable that produces the output you are currently reading.
 4. The Docker daemon streamed that output to the Docker client, which sent it
    to your terminal.

To try something more ambitious, you can run an Ubuntu container with:
 $ docker run -it ubuntu bash

Share images, automate workflows, and more with a free Docker ID:
 https://hub.docker.com/

For more examples and ideas, visit:
 https://docs.docker.com/get-started/

ryusungeun@SungEuns-MacBook-Pro ~ % 
