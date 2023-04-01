# Assignment: Introduction to Docker

## Deliverables
- branch named `docker` with pull request to merge with `master` containing the following:
  - edits to this `README.md` with answers to the questions denoted with `Q:`

## Background

For this assignment you will learn a little about Docker. Docker is a containerization platform designed to isolate and reduce tasks in a way that allows them to be run anytime, anywhere. This assignment follows an online tutorial that describes building and running docker containers in a local environment. However, since we are doing this in Codespaces, there are some important details that you should be aware of. In this sense, this assignment is giving you practice with docker AND codespaces.

### 1. Watch the following overview of what docker is and how it works: https://www.youtube.com/watch?v=YFl2mCHdv24

### 2. Read https://www.docker.com/resources/what-container

### 3. Follow an online tutorial. 
You will follow parts 1-5 of https://docs.docker.com/get-started/ and answer some questions. However...

This part is where some important details differ between the tutorial and codespaces that I wanted to share. So before you get into the tutorial, read some background:

As you know after watching the video and reading the document above, docker allows you to run an image on some client. When it's running it's called a container. The docker images tend to be small, self-contained, and have a single purpose. That is, no extra fluff. Unlike a laptop where you have all your applications installed, a docker image only has what it needs for that one purpose installed. So as long as you have a Docker Engine running, you can run the image. The tutorial assumes you are running docker on your own machine and there will occasionally be instructions that have tabs for `Linux/Mac` vs `Windows`. For running in codespace, you will use the `Terminal` window and follow the instructions for `Linux/Mac` which should be what is shown by default.

There are some specific parts of the tutorial that also need clarification or context.

#### General guidance
All commands should be entered in the `Terminal` window and you should follow the `Linux/Mac` or `CLI` option where there is a code block section in the tutorial.

All references in the tutorial to paths will be relative to the `getting-started` directory and need to be updated accordingly. 

#### In Part two - Get the App
- In step 1, where you clone the `getting-started` repo, enter that command in the `Terminal` window of your Codespace. In fact, all commands should be entered in the `Terminal` window.
- In step 2, the screenshot shows you what this would look like if you opened up the `getting-started` repo in VS Code. Your Codespace will actually look very similar but the `getting-started` repo will actually just look like another directory in your Explorer window:

![./media/vscode-explorer-getting-started.png](./media/vscode-explorer-getting-started.png)

#### In Part two - Build the app's container image,
- `cd /path/to/app` should be changed to `cd getting-started/app` (this applies elsewhere when you see `/path/to/app`)
- `touch Dockerfile` will create a file named `Dockerfile` that will appear in the `getting-started/app` directory in your `Explorer` window. 
- When you open Dockerfile, VSCode will prompt you to install a Docker extension. Install it.

![./media/vscode-install-docker.png](./media/vscode-install-docker.png)

#### In Part two - Start an app container
- Follow the `CLI` options for the commands. I will go over in class how to do the same things using the Docker extension in VSCode. 
- When you run the command `docker run -dp 3000:3000 getting-started`, you will get a VSCode dialog about port 3000. Click the button to open the browser.

![./media/vscode-port-3000-open.png](./media/vscode-port-3000-open.png)

#### In Part three - update the source code
- the path `src/static/js/app.js` refers to the path inside `getting-started`.

#### Do it!
With that out of the way, go ahead and read Parts 1-5 of https://docs.docker.com/get-started/. You can follow along and create your own docker container, which will be part of the assignment below.

## Assignment
Save your work files to a new branch named `solution` and submit a Pull Request to merge with `master` when you are finished but _do not merge_. 

Follow Parts 1-5 of the getting started tutorial at https://docs.docker.com/get-started/.

Answer the following questions in this document:

1) What is your docker username? Put it in the same line as `DOCKER_USER=` below (no markdown please) like `DOCKER_USER=your_username`:

DOCKER_USER=

2) What is docker (your own words)?

A: 

3) What is a docker container?

A: 

4) What is a docker image?

A: 

5) What is a docker volume?

A: 

6) In a Dockerfile, what does `FROM` mean?

A: 

7) In a Dockerfile, what does `EXPOSE` mean?

A: 

8) What is port-forwarding?

A: 

9) What is a docker tag?

A: 

10) What is a docker layer?

A: 

11) What is the difference between a docker tag and docker container id?

A: 

12) What is the difference between a docker hub, repository, and image?

A: 

13) What is detached mode?

A:

14) What is the name of the docker container you created in the tutorial? It should be something like `<your_username>/get-started:part2)` where `<your_username>` is your username. If you have tagged and published (`push`ed) the docker container you created in Part 2, then I will be able to `pull` your container and `run` it on my own machine.

A: 

### Turn in your work via GitHub Pull Request. 

Open a *Pull request* to merge your assignment files with the `master` branch. Do not Merge.
