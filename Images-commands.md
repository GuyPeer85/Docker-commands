# Images commands:

## Defulte command line = "docker < Command > < -Flag > < Image name >":

**`build`**: Builds an image from a Dockerfile.
- `-t`: Tags the image with a name and an optional tag.
- `-f`: Specifies the Dockerfile to use for building the image.
- `--no-cache`: Skips the cache when building the image.

**`pull`**: Pulls an image or a repository from a registry.
- `--all`-tags: Downloads all tags from the repository.
- `--disable-content-trust`: Disables image verification.
- `--platform`: Specifies the platform of the image to pull.

**`push`**: Pushes an image or a repository to a registry.
- `--all-tags`: Pushes all tags associated with the image to the repository.
- `--disable-content-trust`: Disables image verification.
- `--platform`: Specifies the platform of the image to push.

**`rmi`**: Removes one or more images.
- `-f` or `--force`: Forces the removal of an image even if it has dependent child images or running containers.
- `-no-prune`: Prevents Docker from automatically removing untagged parent images.
- `-q` or `--quiet`: Shows only the image IDs (useful for scripting).

**`images`**: Lists all images on the host.
- `-a` or `--all`: Shows all images (including intermediate images).
- `--filter`: Filters the output based on specific conditions (e.g. dangling images, label).
- `--format`: Specifies a custom format to use for the output (in Go template format).

**`commit`**: Creates a new image from a container's changes. It allows you to save the container current state as a new image.
- `-a` or `--author`: Specifies the author name for the new image.
- `-c` or `--change`: Applies changes to the container's file system before committing.
- `-m` or `--message`: Specifies a commit message for the new image.

**`tag`**: This command creates a new tag for an existing image.
- `--force`: Forces the creation of a new tag even if one already exists with the same name.
- `--reference`: Specifies an alternative name reference for the image tag.
- `-f` or `--file`: Specifies the Dockerfile location (for building an image from a Dockerfile).

**`save`**: This command saves one or more images to a tar archive.
- `-o` or `--output`: Specifies the output file name or path.
- `--quiet` or `-q`: Shows only the image IDs (useful for scripting).
- `--tag` or `-t`: Specifies the name and tag for the image(s) to save.

**`load`**: This command loads one or more images from a tar archive.
- `--input` or `-i`: Specifies the input file name or path.
- `--quiet` or `-q`: Shows only the image IDs (useful for scripting).
- `--all-tags` or `-a`: Loads all tags from the tar archive.

**`history`**: This command shows the history of an image.
- `--human`: Shows the sizes and dates in human-readable format.
- `--no-trunc`: Shows the full command in the history (useful for troubleshooting).
- `-H` or `--format`: Specifies a custom format to use for the output (in Go template format).

**`export`**: This command exports the contents of a container's filesystem as a tar archive.
- `-o` or `--output`: Specifies the output file name or path.
- `--quiet` or `-q`: Shows only the container ID (useful for scripting).
- `--change` or `-c`: Applies changes to the container's file system before exporting.
