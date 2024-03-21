# Get started

- Install WSL 2 https://learn.microsoft.com/en-us/windows/wsl/install
- Install Docker Desktop https://www.docker.com/products/docker-desktop/

## Configuration

- In Docker Desktop, enable WSL integration

  - ⚙️ → Resources → WSL integration → Enable integration with my default WSL distro

- Put the docker-compose.yml file in WSL. I have cloned this repository to the following location: `\\wsl.localhost\Ubuntu\home\code-day-2-2024`.

## Let's go!

- Navigate to the directory where you placed your docker-compose.yml file and run the command `docker-compose up -d` using your Ubuntu shell.
- After some startup time you can view the data explorer here: `https://localhost:8081/_explorer/index.html`.

## Extra

### Install mongosh

- Install mongosh: https://www.mongodb.com/try/download/shell
- Navigate to `<PATH>\mongosh-2.1.4-win32-x64\mongosh-2.1.4-win32-x64\bin>`
- Run `mongosh "<MONGO_CONNECTION_STRING>&retryWrites=false" --tlsAllowInvalidCertificates`

  - Example: `mongosh "mongodb://localhost:C2y6yDjf5%2FR%2Bob0N8A7Cgv30VRDJIWEHLM%2B4QDU5DE2nQ9nDuVTqobD4b8mGGyPMbIZnqyMsEcaGQy67XIw%2FJw%3D%3D@localhost:10255/admin?ssl=true&retryWrites=false" --tlsAllowInvalidCertificates`

- Try to add some things to the database. See https://www.w3schools.com/mongodb/mongodb_mongosh_create_database.php
