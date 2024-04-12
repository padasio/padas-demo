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
│   ├── quick-start.yml
│   ├── start-services.yml
│   └── stop-services.yml
└── roles
    ├── kafka
    │   ├── tasks
    │   │   ├── start-broker.yml
    │   │   ├── start-controller.yml
    │   │   ├── stop-broker.yml
    │   │   └── stop-controller.yml
    │   └── vars
    │       └── all.yml
    ├── padas-engine
    │   ├── tasks
    │   │   ├── create_pipeline_bulk.yml
    │   │   ├── create_rules_bulk.yml
    │   │   ├── create_tasks_bulk.yml
    │   │   ├── create_topics.yml
    │   │   ├── create_topologies_bulk.yml
    │   │   ├── get_tokens.yml
    │   │   ├── request.yml
    │   │   ├── start.yml
    │   │   └── stop.yml
    │   └── vars
    │       ├── PadasQuickStartPipelines.json
    │       ├── PadasQuickStartRules.json
    │       ├── PadasQuickStartTasks.json
    │       ├── PadasQuickStartTopologies.json
    │       └── all.yml
    └── padas-ui
        ├── tasks
        │   ├── start.yml
        │   └── stop.yml
        └── vars
            └── all.yml
```

Testing on localhost:

ansible-playbook --connection=local -i inventories/production/group_vars/all.yml  playbooks/quick-start.yml
