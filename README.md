# keycloak-traefik-docker-swarm
#### keycloak with Let's Encrypt in a Docker Swarm


#### Create a secret for storing the password for MySQL root using the command:

#### <pre><code> printf "YourPassword" | docker secret create keycloak-postgres-password -</code></pre>

#### Create a secret for storing the password for WordPress database using the command:

#### <pre><code> printf "YourPassword" | docker secret create keycloak-application-password  - </code></pre>

#### Clear passwords from bash history using the command:

#### <pre><code> history -c && history -w </code></pre>

#### Deploy keycloak in a Docker Swarm using the command:

#### <pre><code> docker stack deploy -c keycloak.yml wordpress</code></pre> 