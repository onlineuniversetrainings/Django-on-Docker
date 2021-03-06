# Django-on-Docker
Get Django on Docker working Locally
Don't have docker installed? Go through this post.

1. Verify Docker Install
Open up terminal (Mac) or PowerShell (Windows)

Copy
$ docker --version
Docker version 19.03.2, build 6a30dfc
2. Build your project's image.
Navigate to your project

Copy
$ cd path/to/your/dev/folder/
$ cd docker_demo
$ ls
Dockerfile  Pipfile     README.md   manage.py
LICENSE     Pipfile.lock    cfehome 
Run the docker build command

Copy
docker build -t demo -f Dockerfile .
Of course the line demo is custom. Change yours if you want.

3. Run a container
Copy
docker run -it -p 8888:8888 demo
Open http://localhost:8888

