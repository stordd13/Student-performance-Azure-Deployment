## End to End Machine Learning Project with Azure Deployment

- Create a container registry in Azure "container"  (Enable the admin user if you want to have credentials to log in)
- Build the docker image and push it to the container registry : 
        - docker build -t container.azurecr.io/your_image_name:latest .   
        - docker login container.azurecr.io  
        - docker push container.azurecr.io/your_image_name:latest
- Then you can create a web app using the image that is now in your Azure container registry
- You can also add Github Action for Continuous Deployment in the Deployment center of you Azure web app. 


Shoutout to Krish Naik from whom this tutorial comes from. My first step into the MLOps field is from him so go check his github:  https://github.com/krishnaik06