## Deployment on EC2

1. Set up the exact folder structure in EC2.
2. Populate the `.env` file with the variables specified in `.env.example` file

Note:

- Make sure to run `docker compose build` everytime you change `nginx.conf` to ensure the nginx server gets updated with the changes.
