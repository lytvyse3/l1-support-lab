#Goals 
- Prepare useful tools for 1st line support
- Practice deploying these tools and monitoring the infrastructure
- Document everything for future reference and potential reuse

#Tools used
| Area                  | Tool                  | Purpose                                      |
|-----------------------|-----------------------|----------------------------------------------|
| Service Desk / ITSM   | GLPI                  | Tickets, SLA, asset inventory                |
| Directory services    | Active Directory      | Users, groups, GPO, domain-joined clients    |
| Remote support        | RustDesk              | Remote access to user machines               |
| Credential management | Passbolt              | Shared team passwords, access control        |
| Monitoring            | Zabbix                | Host monitoring and alerting                 |
| Knowledge base        | BookStack             | Procedures and how-to articles               |
| Backup                | Restic / Veeam        | Backups of VMs and service data              |

#Host machine
- CPU: AMD Ryzen 5 2600X
- RAM: 32GB DDR4
- Storage: 2x 1TB NVMe
- GPU: GTX 1080Ti (planned local LLM with agents)
- OS: Fedora Workstation / Server
- Management: Cockpit
- Virtualization: KVM

#Implementation roadmap
- [ ] Install Fedora, enable Cockpit
- [ ] Deploy Active Directory (domain, OUs, groups, basic GPO)
- [ ] Join Windows clients to the domain
- [ ] Deploy GLPI and configure ticket categories, SLA, asset inventory
- [ ] Deploy RustDesk
- [ ] Deploy Passbolt and set up team access
- [ ] Deploy Zabbix add agents and alerts
- [ ] Set up BookStack with L1 procedures
- [ ] Configure backups and test a restore

#Documentation
Step-by-step guides, configs and screenshots will be stored in the `/docs` folder.
