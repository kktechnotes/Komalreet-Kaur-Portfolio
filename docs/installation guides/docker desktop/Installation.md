# Installing Docker Desktop on Windows - Detailed Guide
The following tasks must be completed in the listed order:

## Step 1: Download and Install Docker Desktop on Windows through GUI
1. Download [Docker Desktop](https://desktop.docker.com/win/main/amd64/Docker%20Desktop%20Installer.exe) for Windows installer.
2. Double-click the installer package to run the installer.
3. On the **Configuration** page, select **Enable WSL 2 Windows Feature** and then click **OK**. The installation component and its dependencies get automatically installed.
4. After installation, click the **Close and Log out** button. The installer application is closed and the current user is logged out.
> **Note**: After installation, you may choose to restart the system.

## Step 2: Check Docker Version and Open the Docker Desktop Application
1. Open **Windows PowerShell** on your system.
2. Type or copy/paste the following command:
    ```
    docker --version
    ```
    **Result**: The response displays the version of the docker. <br/>
    
    > **Note**: In case the installation fails or docker is not completely installed, an error message, "The term 'docker' is not recognized" is displayed. Try to re-install the docker installer package.
 3. Press the Windows key and type, "Docker Desktop" in the search field.
 4. Open the application. The Service Agreement pop-up window is displayed.
 5. Review the [Service Agreement](https://docs.docker.com/subscription/#docker-desktop-license-agreement) and select the "I accept the terms" checkbox.
    ![Agreement](./docker_images/Aggreement.png)
 6. Click **Accept**. Docker starts running and a message, "Docker is running" is displayed.
 > **Tip**: You can also check the docker status from the **Show hidden icons** widget located on the bottom-right of taskbar.
 >          ![docker running](./docker_images/docker%20running.png)

## Step 3: Run Sample Tutorial using Docker
1. Open **Windows PowerShell** on your system.
2. Type or copy/paste the following command:
   ```
   docker run -dp 80:80 docker/getting-started
   ```
   **Result**: A unique container ID is created. <br/>
   
   > **Note**: Refer the [Troubleshooting](./troubleshoot.md) section if you get an error response, "Ports are not available."


> **Next Page**: [Lab](./Lab-run.md)
