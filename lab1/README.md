# Lab 1 
Reference notes and commands from Lab 1.

### 1. Node
   1. Create key pair and save. `swarch-labs.pem`
   2. Connect to instance via ssh
      ```
      % ssh -i "swarch-labs.pem" ubuntu@ec2-18-206-92-20.compute-1.amazonaws.com
      ```

### 2. Docker
   1. Clone test repo and go to directory
      ```
      git clone https://github.com/dockersamples/node-bulletin-board
      cd node-bulletin-board/bulletin-board-app
      ```
   2. Build image
      ```
      docker build --tag bulletinboard:1.0 .
      ```
   3. Run image as container
      ```
      docker run --publish 8000:8080 --detach --name bb bulletinboard:1.0
      ```
   4. Check application in a browser
      ```
      curl localhost:8000
      ```
   5. Delete container (`--force` stops a running container)
      ```
      docker rm --force bb
      ```


### 3. **SHUTDOWN INSTANCE**

