# Elastic Cloud Enterprise Fundamentals

## ECE Architecture

- **Runners**
  - Runners are supervisors on a single machine
  - Runners are assigned one or more roles
  - Runners ensure all container for that role are online and healthy
- **Roles**
  - Roles map to one or more containers
  - **Proxy Role**
    - Handles user requests
    - Keeps track of available of cloud assets
    - Helps with downtime scaling and upgrades
  - **Allocator Role**
    - Must run all all instances where Elastic & Kibana are on
    - Create new containers and start Elastic & Kibana nodes when requested
  - **Coordinator Role**
    - Simply a scheduler that monitors request for Cloud UI, Admin API, ZooKeeper & Director
  - Director Role
    - Manages the distributive data store, data about the infrastructure.

