# StackportDown
StackportDownproject



# stackport_processor

Automates processing of ServiceNow staging records:
- Picks Assigned records → marks WIP → runs device checks (Cisco IOS)
- Decides final status (TRANSFER/CLOSED) based on reachability/stack status
- Updates staging & incident; sends SCON email if TRANSFER

## Prerequisites

- Ansible 2.14+ (or compatible)
- Collections:
  ```bash
  ansible-galaxy collection install -r requirements.yml