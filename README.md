## End to End Machine Learning Project with Azure Deployment

- 1. Create a container registry in Azure "container"  (Enable the admin user if you want to have credentials to log in)
- 2. Build the docker image and push it to the container registry : 
        - docker build -t container.azurecr.io/your_image_name:latest .   
        - docker login container.azurecr.io  
        - docker push container.azurecr.io/your_image_name:latest
- 3. Then you can create a web app using the image that is now in your Azure container registry
