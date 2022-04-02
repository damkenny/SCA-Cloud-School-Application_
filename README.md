# SCA-Cloud-School-Application

Steps Taken to Implement the Assessment.

Step 1: Created a react app and run using the script below

    npx create-react-app newscapp:dev2
    cd myapp
    npm start
    
![image](https://user-images.githubusercontent.com/50354600/161383838-4ceddfeb-92b7-428f-be6d-db47ce8e9226.png)

Step 2: Dockerized the application using docker commands below to test the docker image created and run container.

      docker build --tag newscapp:dev2  .
      docker image ls
      docker run -d -p 3000:3000 newscapp:dev2
      docker ps
![image](https://user-images.githubusercontent.com/50354600/161384562-23e5b7ad-d20d-4061-835c-e16b335841d5.png)

Step 3: Pushed to GitHub Repository with the below git commands into a branch called "Start".

    git checkout -b Start
    git add .
    git commit -m "pushing to start branch"
    git add remote origin https://github.com/damkenny/SCA-Cloud-School-Application.git
    git push -u origin Start

Step 4

a: Made changes on the application file App.js

b: Rebuild the image and run the container using the below commands.

         docker  build -t mynewscapp2:dev3 .
         docker image ls
         docker run -it -p 3000:3000 mynewscapp2:dev3

![image](https://user-images.githubusercontent.com/50354600/161385646-a85b3380-8809-4ddc-a6db-ed217d2bae56.png)

c: pushed to a new branch "feature" and Merge the feature branch to the Start branch.

    git checkout -b feature
    git add .
    git commit -m "pushing to feature branch"
    git push -u origin feature
    git checkout Start
    git merge feature
    
  Step 5: Pushed to dockerhub repository.
  
      docker login
      docker images
      docker tag mynewscapp2:dev3 kehindeafuat/scahub1 
      docker push kehindeafusat/scahub1
  ![image](https://user-images.githubusercontent.com/50354600/161388795-22b0c03e-1897-4214-b59d-85cf354d7250.png)

     
      https://hub.docker.com/repository/docker/kehindeafusat/scahub1
      


  https://hub.docker.com/repository/docker/kehindeafusat/scahub1
  
  
    
