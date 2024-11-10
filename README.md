# Streamlit app with Docker

This is a simple scaffold project of a Streamlit app with a Docker container.

## How to use it

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/streamlit-app-with-docker.git
    ```
2. Navigate to the project directory:
    ```bash
    cd streamlit-app-with-docker
    ```
3. Build the docker image:
    ```bash
    docker compose build 
    ```
4. Run the docker container:
    ```bash
    docker compose up
    ```
5. Your application will be available at http://localhost:8501.

## Useful Docker commands

- List the docker containers: `docker ps`
- Stop the docker container: `docker compose down`
- List the docker images: `docker images`
- Remove the docker image: `docker rmi my-streamlit-app`

## How is this project structured?

- `app/`: contains the Streamlit app.
- `Dockerfile`: the dockerfile to build the docker image.
- `docker-compose.yml`: the docker compose file to run the docker container.
- `.dockerignore`: the docker ignore file to ignore the files that are not needed to be copied to the docker image.
- `requirements.txt`: the dependencies for the project.
- `README.md`: this file.
- `.gitignore`: the git ignore file to ignore the files that are not needed to be committed.


## Steps to recreate the project
1. Create the boilerplate files:
    1. `.gitignore` (from github's Python.gitignore: https://github.com/github/gitignore/blob/main/Python.gitignore):
        ```bash
        curl https://raw.githubusercontent.com/github/gitignore/main/Python.gitignore > .gitignore
        ```
    2. `requirements.txt`
        ```bash
        echo streamlit > requirements.txt
        ```
    3. `README.md`
        ```bash
        echo "# Streamlit app with Docker" > README.md
        ```
    4. `app/streamlit_app.py`
        ```bash
        echo import streamlit as st > app/streamlit_app.py
        ```
2. Initialize a docker project:
    ```bash
    docker init
    ```
3. Change Dockerfile and docker-compose.yml to your needs.
4. Initialize a git repository and add the files:
    ```bash
    git init
    git add .
    git commit -m "Initial commit"
    ```

