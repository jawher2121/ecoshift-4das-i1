# Backend workspace

Create one minimal Spring Boot project per confirmed business service. Keep these as starter projects through Validation 1. Use the Java, Spring Boot, Spring Cloud, and build-tool versions given in class. If the team uses Maven, keep each generated Maven wrapper in Git.

Suggested project paths, subject to the instructor’s service allocation decision:

- `Backend/event-requests/`
- `Backend/stock-and-reservations/`
- `Backend/kit-circulation/`
- `Backend/kit-recovery/`
- `Backend/capacity-planner/`

From an initialized Maven project’s folder in PowerShell, run:

```powershell
.\mvnw.cmd verify
.\mvnw.cmd spring-boot:run
```

Check that the build passes and Spring reports that the application started. Stop with Ctrl+C. Record the actual check and commit under your own account. A database-dependent starter needs its documented local prerequisites before startup can be verified.
