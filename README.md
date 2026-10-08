## Deployment on EC2

1. Set up the exact folder structure in EC2.
2. Populate the `.env` file with the variables specified in `.env.example` file
3. Populate `server.crt` with a signed certificates and `server.key` with a private key. The files are injected into environment running the nginx server via volumes. The nginx server uses the .crt and .key files to set up TSL/SSL.

Note:

- Make sure to run `docker compose build` everytime you change `nginx.conf` to ensure the nginx server gets updated with the changes.
