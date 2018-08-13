# WS Automation

## ansible playbooks for automating WS deployments and various utilities
```
├── dev
├── list_apps.yaml
├── prod
├── qa
├── rc_sch_deply.yaml
├── README.md
├── roles
│   ├── list_apps
│   │   ├── defaults
│   │   │   └── main.yaml
│   │   └── tasks
│   │       └── main.yaml
│   ├── slack
│   │   ├── defaults
│   │   │   └── main.yaml
│   │   └── tasks
│   │       └── main.yaml
│   ├── was_deploy
│   │   ├── defaults
│   │   │   └── main.yaml
│   │   └── tasks
│   │       └── main.yaml
│   ├── was_sync
│   │   ├── defaults
│   │   │   └── main.yaml
│   │   └── tasks
│   │       └── main.yaml
│   └── was_uninstall
│       ├── defaults
│       │   └── main.yaml
│       └── tasks
│           └── main.yaml
├── slack.yaml
├── uat
└── was_sync.yaml

16 directories, 19 files
```

## example playbooks
```
---
- name: wsadmin poc
  hosts: all
  gather_facts: false
  roles:
    - list_apps
```