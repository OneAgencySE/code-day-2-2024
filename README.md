# Get started

- Install WSL 2 https://learn.microsoft.com/en-us/windows/wsl/install
- Install Docker Desktop https://www.docker.com/products/docker-desktop/

## Configuration

- In Docker Desktop, enable WSL integration

  - ⚙️ → Resources → WSL integration → Enable integration with my default WSL distro

- Put the docker-compose-yml file in WSL. I have cloned this repository to the following location: `\\wsl.localhost\Ubuntu\home\code-day-2-2024`.

## Let's go!

- Navigate to the directory where you placed your docker-compose.yml file and run the command `docker-compose up -d` using your Ubuntu shell.
- After some startup time you can view the data explorer here: `https://localhost:8081/_explorer/index.html`.

## Extra

### Install mongosh

- Install mongosh: https://www.mongodb.com/try/download/shell
- Navigate to `<PATH>\mongosh-2.1.4-win32-x64\mongosh-2.1.4-win32-x64\bin>`
- Run `mongosh "mongodb://localhost:<MONGO_TOKEN>@localhost:10255/admin?ssl=true&retryWrites=false" --tlsAllowInvalidCertificates`

- Try to add some things to the database. See https://www.w3schools.com/mongodb/mongodb_mongosh_create_database.php
