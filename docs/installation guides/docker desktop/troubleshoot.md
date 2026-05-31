# Troubleshooting Steps
This section explains how to troubleshoot plausible errors that can occur during installation or while running sample application

## Remapping the Local Port to run Container Images
While running the container images using the command `docker -dp 80:80 getting-started`, you may encounter an error, "Ports are not available." 
![troubleshoot_error](./docker_images/troubleshoot.png)

Docker uses the following port mapping syntax `<your local port>: <docker container image>`. This error may occur because some other application is exposed on the local port. Try to map the local port to some alternate port. <br/>
**Example**:
`docker -dp 89:80 getting-started`

![troubleshoot_solution](./docker_images/troubleshoot-solution.png)

## Docker Desktop is Stopping
After installation of Docker Desktop, on opening the application, you may encounter an error, "Docker Desktop stopping.." 

![docker_stop](./docker_images/Troubleshoot_WSL.png)
This error may occur if the [preinstallation tasks](./Preinstallation.md) are not completed. For example, WSL version 2 is not installed on the system. Review the preinstallation tasks mentioned in the documentation.

![troubleshoot_solution](./docker_images/troubleshoot-solution2.png)

## Sample Application not Running on Localhost
After you try to run the sample application using localhost, you may not be able to view the application and encounter an error, "This page isn’t working". 
The following table describes the possible reasons for this error and its solution:
|          Error Reason           |  Solution                  | 
|---------------------------------|----------------------------|
| Incorrect Docker file name      |  The file name should be `Dockerfile` with no extension|          
| Incorrect Docker File Location  |  The file should be placed inside the app folder|  
