# PLTrust 🛡️  
> *Security enforcement for PL/SQL — natively in your CI/CD pipeline.*

---

## 🔐 Purpose

**PLTrust** is the security pillar of the `PLT*` suite — empowering real DevSecOps for Oracle PL/SQL.  
While `PLTelemetry` observes, and `PLTestLab` verifies, **PLTrust protects**. It brings proactive, automated, policy-driven security validation into your development and deployment lifecycle.

In legacy stacks, security often arrives too late.  
PLTrust shifts it **left** — embedding it natively into your Git workflow, CI/CD pipelines and observability fabric.

---

## 🧠 Key Capabilities

- **Static code analysis (SAST)** for high-risk SQL, dynamic execution, and privilege escalation patterns
- **Security policy enforcement** via customizable rulesets (`no-network`, `no-public-grant`, etc.)
- **Automated checks on PL/SQL packages, procedures, DDL scripts and grants**
- **CI/CD integration** with proper exit codes and inline annotations for pull/merge requests
- **Native telemetry export to `PLTelemetry`** for compliance monitoring and risk traceability
- **Full suite correlation** with `PLTestLab` for audit-linked test enforcement

---

## 🚦 Designed for Pipelines

Whether you're deploying to dev, UAT, or production, PLTrust:

- Executes in **pre-merge or post-build** stages
- Validates all security rules declared for the target environment
- Fails fast and explains why
- Sends structured results to observability pipelines, dashboards or reporting layers

```bash
pltrust run --target ./packages/ --env UAT --ruleset strict.json
