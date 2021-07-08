# MMS Infrastructure

## Repo structure
  
| Directories       | Files                                                                   | Description                                                                         |
|-------------------|-------------------------------------------------------------------------|-------------------------------------------------------------------------------------|
| docker_files      | docker-compose.yml<br>docker-compose.dev.yml<br>docker-compose.prod.yml | general docker compose yaml file<br>dev specific override<br>prod specific override |
| ansible_playbooks | application_server.yml<br>monitoring_server.yml| Ansible playbooks for setup application and monitorings servers |
