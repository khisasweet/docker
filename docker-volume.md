
Chapter Summary: Volumes and Persistent Data

Summary of the concepts covered in this chapter.
Commands

Let's explore all the commands covered in this chapter:

    docker volume create creates new volumes. By default, it creates them with the local driver, but you can use the -d flag to specify a different driver.

    docker volume ls lists all volumes on your Docker host.

    docker volume inspect shows you detailed volume information. You can use this command to see where a volume exists in the Docker host’s filesystem.

    docker volume prune deletes all volumes not in use by a container or service replica. Use with caution!

    docker volume rm deletes specific volumes that are not in use.

Quick recap

There are two main types of data: persistent and non-persistent.

    Persistent data is data you need to keep, and non-persistent data is data you don’t need to keep.

    By default, all containers get a layer of writable, non-persistent storage that lives and dies with the container. We sometimes call this local storage, and it’s ideal for non-persistent data. However, if your apps create data you need to keep, you should store the data in a Docker volume.

    Docker volumes are first-class objects in the Docker API, and you manage them independently of containers using their own docker volume sub-command. This means deleting containers doesn’t delete the data in their volumes.

    A few third-party plugins exist that provide Docker with access to specialized external storage systems.

    Volumes are the recommended way to work with persistent data in Docker environments.
