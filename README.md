# padas-demo

```
.
├── README.md
├── inventories
│   └── production
│       ├── group_vars
│       │   ├── all.yml
│       │   ├── kafka.yml
│       │   ├── padas-engine.yml
│       │   └── padas-ui.yml
│       └── host_vars
│           ├── kafka.yml
│           ├── padas-engine.yml
│           └── padas-ui.yml
├── playbooks
│   ├── getting-started.yml
│   ├── start-services.yml
│   └── stop-services.yml
└── roles
    ├── common
    ├── kafka
    │   ├── handlers
    │   ├── tasks
    │   └── vars
    ├── padas-engine
    │   ├── handlers
    │   ├── tasks
    │   │   ├── start.yml
    │   │   └── stop.yml
    │   └── vars
    │       └── all.yml
    └── padas-ui
        ├── handlers
        ├── tasks
        │   ├── start.yml
        │   └── stop.yml
        └── vars
            └── all.yml
```

Testing on localhost:

ansible-playbook --connection=local -i inventories/production/group_vars/all.yml  playbooks/start-services.yml
ansible-playbook --connection=local -i inventories/production/group_vars/all.yml  playbooks/stop-services.yml