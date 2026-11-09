# EcoShift

EcoShift is an ESPRIT Distributed Web Applications design proposal for reusable event supplies. Club organizers request cups and trays, coordinators review availability, and stockroom staff track pickup, return, and clearance. Validation scenarios use simulated records for a proposed ESPRIT pilot.

**Class** 4DAS_I 1 · **Group** EcoShift · **Team** Six students. Replace Student A through Student F in the [backlog](Documentation/Backlog.md) with the team’s agreed names before submission.

## Validation 1 materials

- [Presentation](Documentation/Presentation/EcoShift-Session-4.pptx)
- [Technical design](Documentation/EcoShift-Technical-Design.docx)
- [Overall architecture](Documentation/Diagrams/Architecture.svg)
- [Use cases](Documentation/Diagrams/Use-Cases.svg)
- [Approval sequence](Documentation/Diagrams/Approval-Sequence.svg)
- [Return and recovery sequence](Documentation/Diagrams/Return-Recovery-Sequence.svg)
- [Domain class diagrams](Documentation/Diagrams/Domain-Classes.md)
- [Backlog, owner slots, and acceptance criteria](Documentation/Backlog.md)

## Repository and project status

```text
Backend/                     Confirmed Spring Boot projects go here
Frontend/                    Shared client workspace
Documentation/
  Presentation/
  Diagrams/
  EcoShift-Technical-Design.docx
  Backlog.md
README.md
```

The design proposes Event Requests, Stock and Reservations, Kit Circulation, Kit Recovery, and the shared Capacity Planner. Their databases are isolated. Spring Cloud Gateway, Eureka, Config Server, Keycloak, RabbitMQ, and Docker Compose are planned shared infrastructure. The grading model for six students is pending instructor confirmation.

This repository starts with the design materials. The team adds verified starter projects after confirming service ownership. Each owner compiles and starts their own project and commits their contribution. See [Backend setup](Backend/README.md) for the planned verification commands.

## Git workflow

Use a GitHub issue for each backlog item and put it on a GitHub Projects board with its owner, dependencies, and acceptance criteria. Work on a short branch, link the pull request to the issue, and ask a teammate to review before merging to `main`. Add the instructor as a collaborator and check the public links before the presentation.
