Chapter Summary: Docker Security

Summary of the concepts covered in this chapter.
Commands

Let's explore all the commands covered in this chapter:

    docker scout provides insights and recommendations for optimizing container images and improving security. It helps identify vulnerabilities and suggests improvements.

    docker swarm update updates services in a Docker Swarm cluster, enabling configuration changes to run services without downtime.

    docker secrets securely manages sensitive data (e.g., passwords, API keys) in a Docker Swarm cluster. Secrets are encrypted and only accessible by authorized services.

    docker trust manages image signing and verification to ensure the authenticity and integrity of Docker images, preventing the use of tampered images.

Quick recap

    You can configure Docker to be extremely secure. It supports all major Linux security technologies such as kernel namespaces, cgroups, capabilities, MAC, and seccomp. It ships with sensible defaults for all these, but you can customize and disable them.

    In addition to the Linux security technologies, Docker includes an extensive set of its own security technologies. Swarms are built on TLS and are secure out of the box. Docker Scout performs binary-level image scans and provides detailed reports of known vulnerabilities and suggested fixes. Docker Content Trust lets you sign and verify images, and Docker secrets allow you to share sensitive data with swarm services.
