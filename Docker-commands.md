# Docker commands:

## Defulte command line = "docker < Command > < -Flag >":

**`login`**: Log in to a Docker registry.
- `-u` or `--username`: Specify the username to log in with.
- `-p` or `--password`: Specify the password to log in with.
- `--email`: Specify the email address to use for the account.

**`logout`**: Log out from a Docker registry.
- `--all`: Log out from all registries.
- `--password-stdin`: Read the password from stdin.
- `--username`: Specify the username to log out of.

**`info`**: Display system-wide information about Docker.
- `--format`: Specify a custom format to use for the output (in Go template format).
- `-f` or `--filter`: Filter output based on conditions provided.
- `--verbose`: Show detailed information about Docker resources.

**`version`**: Display version information about Docker.
- `-f` or `--format`: Specify a custom format to use for the output (in Go template format).
- `--short`: Show only the version number.
- `--verbose`: Show detailed information about Docker resources.

**`network`**: Manage Docker networks.
- `--driver`: Specify the driver to use for the network.
- `--subnet`: Specify a custom subnet to use for the network.
- `--ip-range`: Specify a custom IP range to use for the network.

**`volume`**: Manage Docker volumes.
- `--driver`: Specify the driver to use for the volume.
- `--label`: Add a label to the volume.
- `--opt`: Specify driver-specific options for the volume.

**`system`**: Manage Docker system resources, such as prune unused data.
- `--force` or `-f`: Force removal of unused Docker resources.
- `--volumes`: Remove unused volumes.
- `--filter`: Provide filter values to prune specific unused Docker resources.

docker-compose: Define and run multi-container Docker applications.
- `-f` or `--file`: Specify the location of the Compose file.
- `-p` or `--project-name`: Specify a custom project name.
- `--verbose`: Show verbose output.
- `--no-ansi`: Disable ANSI color output.
- `--no-build`: Don't build an image, even if it's missing.
- `--no-deps`: Don't start linked services.
- `--force-recreate`: Recreate containers even if their configuration hasn't changed.
- `--build`: Build images before starting containers.
- `--scale`: Set the number of containers to run for a service.
- `--abort-on-container-exit`: Stop all containers if any container stops.
