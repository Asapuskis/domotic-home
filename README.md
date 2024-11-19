# domotic-home
## Running the Project with Docker Compose

To run this project using Docker Compose, follow these steps:

1. **Clone the repository**:
    ```sh
    git clone https://github.com/Asapuskis/domotic-home
    cd domotic-home
    ```

2. **Build and start the containers**:
    ```sh
    docker-compose up -d
    ```

4. **Access the applications**:
    Open your browser and navigate to:
    - `http://localhost:9080/`: [zigbee2mqtt](https://www.zigbee2mqtt.io/)
    - `http://localhost:4000/`: [mqtt-explorer](https://mqtt-explorer.com/) 
    - `http://localhost:1880/`: [node-red](https://nodered.org/docs/)

5. **Stopping the containers**:
    To stop the containers, run:
    ```sh
    docker-compose down
    ```

6. **Additional commands**:
    - To view the logs of a specific service:
      ```sh
      docker-compose logs -f SERVICE_NAME
      ```
    - To run a command inside a running container:
      ```sh
      docker-compose exec SERVICE_NAME COMMAND
      ```

Make sure Docker and Docker Compose are installed on your system before running these commands.