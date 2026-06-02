# Lab: Running Container Image of an Application on Docker Desktop
This section describes the steps to run your first docker application. For demonstration purposes, use the [sample application](https://github.com/docker/getting-started).
> **Assumption**: You are familiar with GIT concepts and GIT is installed on your system.

## Step 1: Clone the Sample Application Repository on your Local System
1. Create a new folder in your local GIT repository.
2. Go to the [sample application](https://github.com/docker/getting-started) repository on GitHub.
3. Go to the **Code** dropdown list and under **HTTPS**, click the copy icon to copy the repository link.
4. Open the local GIT repository and go to the new folder created in step 1 of this task.
5. Open command prompt. <br/>

    > **Tip**: In the file explorer, Select the path in the address bar > Type "cmd"  > Press Enter. 
6. Type `git clone <link to repository>` and press Enter. The system clones the repository successfully.
> **Note**: Alternatively, you can go to the **Code** dropdown list and download the ZIP package.

## Step 2: Create a Docker File
1. Open any text editor, such as *VS Code* or *Notepad ++* and type the following code
   ```
    # syntax=docker/dockerfile:1
    FROM node:12-alpine
    RUN apk add --no-cache python2 g++ make
    WORKDIR /app
    COPY . .
    RUN yarn install --production
    CMD ["node", "src/index.js"]
    EXPOSE 3000
    ```
  2. Save the file with name as `Dockerfile` without any extension and place it inside the **app** folder.

> **Important**: The file name must be `Dockerfile` and must be placed inside the **app** folder.

## Step 3: Build and Tag the Container Image
1. Open "Windows PowerShell" inside the **apps** folder.
2. Type the following command
    ```
     docker build -t komal-getting-started .
    ```

 > **Note**: You can replace "komal-getting-started" with any meaningful name.

 ## Step 4: Run a Container Image of the Sample Application
 1. In the Windows PowerShell, type the following command
     ```
     docker run -dp 90:3000 komal-getting-started
    ```
    A unique container ID is up and running.
     ![run_command](./docker_images/Run_Sample.png)
 2. To check the status, type `docker ps -a`. A list of container images running on the system is displayed.
 3. Open browser and type `http://localhost:90`. The application runs successfully.
![sampleapp](./docker_images/sample%20app.png)

> **Next Page**: [Troubleshooting](troubleshoot.md)
