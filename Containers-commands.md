# Containers commands:

## Defulte command line = docker < Command > < -Flag > < Container Name >:

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

**`create`**: Creates a new container but does not start it.
**`-it`**: Allocates a pseudo-TTY for the container.
- `--name`: Assigns a name to the container.
- `--env`: Sets an environment variable in the container.

**`restart`**: Stops and starts one or more running containers.
- `-t`: Specifies the number of seconds to wait before forcefully stopping the container.
- `-f`: Forces the container to stop immediately.
- `--time`: Specifies a custom timeout value in seconds for graceful stop.

**`pause`**: Pauses all processes within one or more running containers.
- `-t`: Specifies the number of seconds to wait before forcefully pausing the container.
- `-f`: Forces the container to pause immediately.
- `--time`: Specifies a custom timeout value in seconds for graceful pause.

**`inspect`**: Displays detailed information on one or more containers or images.
- `-f`: Specifies a custom format to use for the output.
- `--type`: Specifies the type of object to inspect (container or image).
- `--format`: Specifies a Go template to use for the output.

**`top`**: Displays the running processes within a container.
- `-a`: Shows all processes (including those that have finished).
- `-o`: Specifies the column to sort by (e.g. CPU usage, memory usage).
- `--pid`: Shows processes for a specific PID.
