# padas-demo

ansible/
├── inventories/
│   ├── production/
│   │   ├── group_vars/
│   │   │   ├── all.yml
│   │   │   ├── padas-engine.yml
│   │   │   ├── padas-ui.yml
│   │   │   ├── kafka.yml
│   │   ├── host_vars/
│   │   │   ├── padas-engine.yml
│   │   │   ├── padas-ui.yml
│   │   │   ├── kafka.yml
│   ├── staging/
│   │   ├── group_vars/
│   │   │   ├── all.yml
│   │   ├── host_vars/
│   │   │   ├── staging-server.yml
├── playbooks/
│   ├── padas-engine.yml
│   ├── padas-ui.yml
│   ├── kafka.yml
├── roles/
│   ├── common/
│   │   ├── defaults/
│   │   ├── tasks/
│   │   ├── handlers/
│   │   ├── templates/
│   │   ├── files/
│   │   ├── vars/
│   ├── padas-engine/
│   │   ├── defaults/
│   │   ├── tasks/
│   │   ├── handlers/
│   │   ├── templates/
│   │   ├── files/
│   │   ├── vars/
│   ├── padas-ui/
│   │   ├── defaults/
│   │   ├── tasks/
│   │   ├── handlers/
│   │   ├── templates/
│   │   ├── files/
│   │   ├── vars/
│   ├── kafka/
│   │   ├── defaults/
│   │   ├── tasks/
│   │   ├── handlers/
│   │   ├── templates/
│   │   ├── files/
│   │   ├── vars/