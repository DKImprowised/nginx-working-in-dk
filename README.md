# nginx-working-in-dk

add localhost entries in /etc/hosts file.

127.0.0.1 gitea.localhost
127.0.0.1 hydra.localhost
127.0.0.1 consent.localhost

run hydrastart.yml and hydrastart-postgres.yml compose files

make sure /nginx/conf.d/working.conf file is present inside nginx container's /etc/nginx/conf.d/ directory and also default.conf should not be there.

if you are seeing welcome nginx, that's coming from default.conf, delete it and reload the configurations with working.conf

hit the urls, hydra.localhost, gitea.localhost, consent.localhost and check all are working as expected.
