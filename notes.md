# Docker

### What is it?
 * Similar to a VM
    * Isolation of processes in a secure container
    * But wait, the linux kernel already provides that!
    * Limiting of CPU/resources/disk space
 * Different from a VM
    * Shared kernel
    * Lighter weight
    * Efficiencies e.g. memory space/pressure
 * Comparison to LXC etc
 * Docker hub (lots of prebuilt images, but not all necessarily well-built/secure)

### What isn't it?
 * Full virtualization
 * Necessarily nestable
 * Always secure (docker==sudo, root in container can be root outside with the right container)

### Demos
 * Spin up increasingly complex
   * `sh` in alpine
   * `bash` in ubuntu
   * DTANM (scaling)
 * Different OS userspace (since it's all the same kernel it works)
   * Ubuntu
   * Debian
   * RHEL
   * Arch
   * Manjaro
 * Shared resources
 * Resource limitations
 * Interactivity
 * mysql-client ("don't need to install")
 * 
docker run -e ENV=env --cpus 1 -h hostname -m memory_bytes
 * LXC, if time.

Write myself:
 * echo Hello World
 * Flask app
 * memory limitation
 * Root exploit
 * sudo in container != sudo on host (`rm -rf /`)
### Use
 * Automatically deploying independent services
 * 

### Automation
 * Docker -> docker-compose -> docker swarm -> docker stack -> docker machine
 * K8s/Kubernetes
 * Provides
   * Scaling, both within and outside a host

# Filesystem (Layers)

# Networking
