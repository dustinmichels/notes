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

## Linux Stuff

### Apt

#### Autoremove

> autoremove is used to remove packages that were automatically installed to satisfy dependencies for other packages and are now no longer needed as dependencies changed or the package(s) needing them were removed in the meantime.

    sudo apt autoremove

#### Autoclean

> The apt-get autoclean option, like apt-get clean, clears the local repository of retrieved package files, but it only removes files that can no longer be downloaded and are virtually useless. It helps to keep your cache from growing too large.

    sudo apt autoclean
