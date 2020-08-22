![Express Socket.io](https://miro.medium.com/max/1200/1*tWm33yhceKIL22QqOORu2w.png)

# Hello Chat
Realtime chat app with websockets using Node.js, Express and Socket.io with Javascript on the frontend with a custom UI

## Table of contents

- [Setting up the project](#setting-up-the-project)
- [Setting up the project with Docker](#setting-up-the-project-with-docker)
- [Cleaning up the Container and Image](#cleaning-up-the-container-and-image)
- [Inspiration](#inspiration)
- [Contact](#contact)

## Setting up the project

  Start by cloning the project with the command:
  ```
  $ git clone https://github.com/rmiyazaki6499/hello_chat.git
  ```
  
  ## Setting up the project with Docker

  For those that are not interested in setting up the project manually or would simply not have to worry about downloading node.js and its dependencies, I have created a Dockerfile and docker-compose.yml file to help create a container with everything you would need to run the **hello_chat**.

  ### Install Docker

  To make this as easy as possible, we will be using *Docker Compose* to creat our container.

  - If you do not have Docker yet, start by downloading it if you are on a Mac or Windows:
  https://www.docker.com/products/docker-desktop

  - Or if you are on a Linux Distribution follow the directions here:
  https://docs.docker.com/compose/install/

  - To confirm you have Docker Compose, open up your terminal and run the command below:

  ```
  $ docker-compose --version
  docker-compose version 1.26.2, build eefe0d31
  ```
  
  - Go into the project directory to build and run the container with:

  ```
  $ cd hello_chat/
  $ docker-compose up -d --build
  ```

  **This may take a few moments**
  
  Navigate to http://localhost:3000 to view the site on the local server.
It should look something like this:

![Hello Chat Sign In](https://user-images.githubusercontent.com/41876764/90868239-6ed92b80-e34b-11ea-897f-d1b4f6a5c772.png)

![Hello Chat Chatroom](https://user-images.githubusercontent.com/41876764/90868272-7ac4ed80-e34b-11ea-9dd0-0a08c699c75c.png)
  
  ### Cleaning up the Container and Image

  - To stop the container from running, use `<Ctrl-C>` twice.
  - To close down the container use the command:

  ```
  $ docker-compose down
  ```
  - Then to clean up the container and image which we are no longer using use the command:

  ```
  $ docker system prune -fa
  ```

  - Confirm that the container and image is no longer there with:

  ```
  $ docker system df -v
  ```

## Inspiration

Video Tutorial
https://www.youtube.com/watch?v=jD7FnbI76Hg&feature=youtu.be

Source code
https://github.com/bradtraversy

## Contact

[Ryuichi Miyazaki](https://github.com/rmiyazaki6499)
