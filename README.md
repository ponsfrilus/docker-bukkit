# Docker Bukkit

Forked from https://github.com/bbriggs/docker-bukkit

## A Bukkit/Spigot server on docker
Bukkit, a moddable Minecraft server. On Docker. Neat, huh?


### Running the server
To start the server and accept the EULA in one fell swoop, just pass the `EULA=true` environment variable to Docker when running the container. I recommend mounting a directory from your host onto `/data` in the container to make map and server data persistent.

Example:
`docker run -it -v /data:/data -p 25565:25565  -e EULA=true --name mc_server ponsfrilus/docker-bukkit`
