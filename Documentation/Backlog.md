# EcoShift backlog

Replace Student A through Student F with the six team members’ names. The workstreams are a provisional division of work. Confirm how each student will satisfy the individual service criterion before treating these as graded service assignments.

## Before Validation 1

### V1 Confirm service ownership and topic availability

- **Owner** Student A, with the team
- **Depends on** Instructor and class topic list
- **Acceptance** Record the accepted service count and owners, how the shared planner is presented, and whether the topic is available.

### V2 Verify the public repository

- **Owner** Student E, reviewed by Student F
- **Depends on** Instructor’s GitHub username and team account access
- **Acceptance** Public link works signed out. Required directories and README are present. Instructor collaborator access and the Projects board are visible.

### V3 Initialize and verify confirmed services

- **Owner** Each confirmed service owner
- **Depends on** V1, V2, and the course’s Java and Spring versions
- **Acceptance** Each starter lives under Backend, compiles, and starts. Each owner records their actual build and startup evidence and makes personal Git commits.

### V4 Review diagrams and API contracts

- **Owner** Students A–D for their candidate domains, Student E for integration, Student F for report consistency
- **Depends on** V1
- **Acceptance** Each service has a distinct capability, an owner, a class model, a database rationale, main routes and response codes, and an explained failure case. Diagrams and contracts use the same names.

### V5 Rehearse and prepare Blackboard

- **Owner** Student F coordinates, all six speak, one named teammate submits
- **Depends on** V2–V4
- **Acceptance** Finish a ten-minute talk, keep each personal service segment within one minute, show the actual repository and Git history, and rehearse at least one question per student. The draft includes six names and verified links. Use the active Blackboard assignment.

## After design approval

### B1 Gateway and shared frontend entry point — S5

- **Owner** Student E with the whole team
- **Depends on** V1, V3, and approval
- **Acceptance** A browser request reaches the intended Spring Boot service through Gateway. Direct business API access is unnecessary for the demo.

### B2 Requests and reservations — S6

- **Owner** Students A and B
- **Depends on** B1 and the request and stock contracts
- **Acceptance** An organizer creates a request and a coordinator approves a feasible booking through OpenFeign. Competing approvals cannot reserve more ready stock than exists. A retry reconciles an unknown outcome.

### B3 Pickup, return, and recovery — S7

- **Owner** Students C and D with Student B
- **Depends on** B2
- **Acceptance** An approved booking is issued. A return accounts for intact, damaged, and missing units. Redelivery cannot move stock twice. A cleared lot becomes ready and damaged stock stays unavailable until resolved.

### B4 Shared capacity planner — S7 and S8

- **Owner** Whole team. Student F coordinates the forecast acceptance scenario
- **Depends on** B2 and B3 event contracts
- **Acceptance** PostgreSQL stores its own versioned projections. A simulated overdue return produces a shortage for a future pickup. Forecast downtime does not block approval.

### B5 Keycloak roles and ownership — S8

- **Owner** Student E with all service owners
- **Depends on** B1–B3
- **Acceptance** Club organizers access only their requests, coordinators approve and view forecasts, and staff record pickup and return. Invalid access returns the documented error.

### B6 Compose and defense — S9 and S10

- **Owner** Student E coordinates Compose. Student F coordinates the demo. All six contribute
- **Depends on** B1–B5
- **Acceptance** A clean environment starts from the documented Compose steps. The team can demonstrate request, conflict, handover, return, clearance, and forecast with labeled simulated data. Each member can explain their contribution and a failure scenario.
