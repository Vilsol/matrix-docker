# matrix-docker

Easy to use docker stack for matrix

## Usage

1. Clone this repository
2. Edit `docker-compose.yml`:
    1. Change `YOUR_DOMAIN` to your domain (e.g. matrix.example.com).
    2. Change `CHANGE_DEFAULT_PASSWORD` to some random string.
3. Edit `traefik-data/traefik.toml`:
    1. Change `YOUR_EMAIL` to your email (e.g. user@example.com).
4. Run `docker-compose up -d`
5. Add an SRV record to your domain `_matrix._tcp.YOUR_DOMAIN. SRV 1 1 443 YOUR_DOMAIN.`
6. Test your domain against federation tester: https://matrix.org/federationtester/
