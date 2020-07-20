# Making Space

Dealing with common culprits that take up space on harddrive.

## Anaconda/ Miniconda

### Remove unused packages and caches

    conda clean --all

### Remove unused environments

    # list environments
    conda env list

    # remove environment
    conda remove --name myenv --all

## Docker

### Cleanup dangling resources

> "Docker provides a single command that will clean up any resources — images, containers, volumes, and networks — that are dangling (not associated with a container):"

    docker system prune
