# Docker_Tutorial

Get Docker
------------------
Docker is an open platform for developing, shipping, and running applications. Docker enables you to separate your applications from your infrastructure so you can deliver software quickly. With Docker, you can manage your infrastructure in the same ways you manage your applications. By taking advantage of Docker’s methodologies for shipping, testing, and deploying code quickly, you can significantly reduce the delay between writing code and running it in production.

Why Use Docker?
-------------------
1. Enables Efficient Use Of Resources
2. Faster Software Delivery Cycles
3. Application Portability

Isolate Namespaces in Docker
--------------------------------
* Net: network of every container is isolate
* Pid: proccess of every container is isolate
* Mnt: mountpoint of every container is isolate
* User: Users of every container is isolate
* UTS: Hostname of every container is isolate
* IPC: the process will have an independent namespace for system

cgroups: isolate resources

Docker Engine overview
--------------------------
Docker Engine is an open source containerization technology for building and containerizing your applications. Docker Engine acts as a client-server application with:

* A server with a long-running daemon process dockerd.
*APIs which specify interfaces that programs can use to talk to and instruct the Docker daemon.
* A command line interface (CLI) client docker.

The CLI uses Docker APIs to control or interact with the Docker daemon through scripting or direct CLI commands. Many other Docker applications use the underlying API and CLI. The daemon creates and manage Docker objects, such as images, containers, networks, and volumes.

What is a container?
---------------------------
Containers are great for continuous integration and continuous delivery (CI/CD) workflows.

Now that you’ve run a container, what is a container? Simply put, a container is a sandboxed process on your machine that is isolated from all other processes on the host machine. That isolation leverages kernel namespaces and cgroups, features that have been in Linux for a long time. Docker has worked to make these capabilities approachable and easy to use. To summarize, a container:

* is a runnable instance of an image. You can create, start, stop, move, or delete a container using the DockerAPI or CLI.
* can be run on local machines, virtual machines or deployed to the cloud.
* is portable (can be run on any OS).
* is isolated from other containers and runs its own software, binaries, and configurations.

What is a container image?
-----------------------------
When running a container, it uses an isolated filesystem. This custom filesystem is provided by a container image. Since the image contains the container’s filesystem, it must contain everything needed to run an application - all dependencies, configurations, scripts, binaries, etc. The image also contains other configuration for the container, such as environment variables, a default command to run, and other metadata.


