# padas-demo

padas-demo/
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
├── playbooks/
│   ├── getting-started.yml
│   ├── padas-engine.yml
│   ├── padas-ui.yml
│   ├── kafka.yml
├── roles/
│   ├── common/
│   ├── padas-engine/
│   │   ├── tasks/
│   │   ├── handlers/
│   │   ├── vars/
│   ├── padas-ui/
│   │   ├── tasks/
│   │   ├── handlers/
│   │   ├── vars/
│   ├── kafka/
│   │   ├── tasks/
│   │   ├── handlers/
│   │   ├── vars/
