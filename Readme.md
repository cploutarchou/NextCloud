##  Nextcloud Docker Server with ONLYOFFICE 

## Requirements

* The latest version of Docker (can be downloaded here: [https://docs.docker.com/engine/installation/](https://docs.docker.com/engine/installation/))
* Docker compose (can be downloaded here: [https://docs.docker.com/compose/install/](https://docs.docker.com/compose/install/))


## Installation

1. Get the latest version of this repository running the command:

    ```
    git clone https://github.com/cploutarchou/NextCloud.git
    cd NextCloud
    ```

2. Run Docker Compose:

   **Please note**: the action must be performed with **root** access rights.

    ```
    docker-compose up -d
    ```

   **Please note**: you might need to wait a couple of minutes when all the containers are up and running after the above command.

3. Now launch the browser and enter the webserver address. The Nextcloud wizard webpage will be opened. Enter all the necessary data to complete the wizard.

### Notice: Is required to perform the initial configuration before running the following command 

4. Go to the project folder and run the `set_configuration.sh` script:
   
   **Please note**: the action must be performed with **root** rights.
    ```
    ./init_onlyoffice.sh
    ```
## Additional Notes
* If you select to install the recommended apps please note that you need to disable Collabora plugins to 
be possible onlyoffice to be used as the default document editor. 