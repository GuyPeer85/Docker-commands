# Docker-commands <img src="https://github.com/devicons/devicon/blob/master/icons/docker/docker-original-wordmark.svg" title="Docker" alt="Docker" width="40" height="40" height="40"/>&nbsp;

See all commands / description / exmaples in the md files

Containers commands - docker < command > < -flag >:
-----------------------------------------------
**`run`:** Runs a command in a new container.
- `-d`: Runs the container in detached mode (in the background).
- `-p`: Publishes a container's port(s) to the host.
- `-v`: Mounts a volume from the host to the container.

**`start`:** Starts one or more stopped containers.
- `-a`: Attaches the container's output to the current terminal.
- `-i`: Attaches the container's input to the current terminal.
- `--restart`: Specifies a restart policy for the container.

**`stop`:** Stops one or more running containers.
- `-t`: Specifies the number of seconds to wait before forcefully stopping the container.
- `-f`: Forces the container to stop immediately.
- `--time`: Specifies a custom timeout value in seconds for graceful stop.
  
**`exec`:** Stops one or more running containers.
- `-t`: Specifies the number of seconds to wait before forcefully stopping the container.
- `-f`: Forces the container to stop immediately.
- `--time`: Specifies a custom timeout value in seconds for graceful stop.

**`ps`:** Lists all running containers.
- `-a` or `--all`: Shows all containers (running and stopped).
- `-f` or `--filter`: Filters the output based on specific conditions (e.g. container status, label).
- `-q` or `--quiet`: Shows only the container IDs (useful for scripting).

**`logs`:** Shows logs from a container.
- `-f` or `--follow`: Shows live logs (similar to tail -f).
- `--since` or `--until`: Shows logs within a specific time range.
- `--tail`: Shows a specific number of log lines (default is all).

**`rm`:** Removes one or more containers.
- `-f` or `--force`: Forces the removal of a running container.
- `-v` or `--volumes`: Removes any associated volumes as well.
- `-l` or `--link`: Removes any associated links (deprecated in newer Docker versions).

**`inspect`:** Removes one or more containers.
- `-f` or `--format`: Specifies a custom format to use for the output (in Go template format).
- `--type`: Specifies the type of object to inspect (container or image).
- `--size`: Shows the size of each object in the output (e.g. image layers, container filesystem).
