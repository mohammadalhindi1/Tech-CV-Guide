# Writing Strong Technical Bullet Points

## The core formula

A useful technical bullet often follows:

> **Action + what you built or changed + technology/context + result, scale, or purpose**

Not every bullet needs all four elements, but each bullet should communicate more than a tool name.

## From task to evidence

Weak:

> Responsible for AWS.

Better:

> Deployed a web application on AWS EC2 with application data stored in RDS and static assets in S3.

Better with a real reliability decision:

> Deployed a web application across EC2, RDS, and S3, separating compute, relational data, and object storage to simplify backup and maintenance.

## Four useful types of evidence

### 1. Measurable outcome

> Reduced Docker image size from 780 MB to 460 MB by using a multi-stage build and removing development dependencies.

Use this only when you measured both values.

### 2. Scope or scale

> Implemented 12 REST endpoints covering authentication, enrollment, grade entry, and role-based workflows.

A scope metric is still useful even when there is no business impact metric.

### 3. Technical complexity

> Implemented pipeline execution in a Unix shell using fork, pipe, dup2, execve, and waitpid, including redirection and exit-status handling.

### 4. Quality or validation

> Added GitHub Actions checks for compilation, functional cases, and Valgrind analysis to catch regressions on each push.

## Writing without fake metrics

Many student projects do not have revenue, customers, or production traffic. Do not manufacture impact.

Instead, describe:

- number of endpoints, services, tests, roles, or environments;
- automated steps;
- deployment target;
- supported failure cases;
- security controls;
- validation method;
- performance measured locally with a stated method;
- reliability or maintainability improvement you can demonstrate.

## Use accurate action verbs

Choose the verb that describes your work:

| Intent | Useful verbs |
|---|---|
| Build | built, developed, implemented, created |
| Improve | optimized, reduced, simplified, refactored |
| Operate | deployed, configured, monitored, maintained |
| Automate | automated, scripted, integrated, provisioned |
| Investigate | analyzed, diagnosed, tested, troubleshot |
| Collaborate | coordinated, documented, reviewed, presented |

Avoid replacing clear language with dramatic verbs merely to sound senior.

## Explain the technology's role

Weak:

> Used Docker, AWS, Linux, and GitHub.

Strong:

> Containerized the API with Docker, hosted it on an AWS EC2 Linux instance, and used GitHub Actions to run automated build checks.

The second version shows how the tools connect.

## Separate team output from personal contribution

Ambiguous:

> Built a university registration platform.

Clearer:

> Implemented the deployment workflow and AWS infrastructure for a team-built university registration platform using EC2, RDS, and S3.

Use “collaborated” or “contributed” when appropriate, then state your exact ownership.

## Tense and style

- Use past tense for completed work: **built**, **deployed**, **tested**.
- Use present tense for ongoing responsibility: **maintain**, **monitor**, **support**.
- Start with a verb.
- Remove “I” from bullets.
- Keep one main idea per bullet.
- Avoid ending some bullets with periods and others without them.
- Define uncommon abbreviations once.

## Editing exercise

Original:

> Made a Docker project and used Kubernetes and it was working.

Ask:

1. What was the application?
2. What exactly did Docker package?
3. Where did Kubernetes run?
4. Which resources were created?
5. How was success tested?

Rewritten:

> Containerized a FastAPI task service and deployed it to Minikube using Kubernetes Deployment and Service manifests; verified health and CRUD endpoints through Postman.

The rewritten bullet is stronger because it is specific and interview-ready, not because it uses more impressive vocabulary.
