# Mandas

**Stop emailing banks to test your integrations.**

Mandas is an open source payment simulation platform for fintech and banking 
engineering teams. Test the full lifecycle of SEPA and SWIFT transactions — 
including R-transactions, returns, rejects, and failures — without waiting for 
a bank to respond.

## The problem

Every fintech team hits the same wall: bank sandboxes cover happy paths. The 
moment you need to trigger a return, a reject, or a mandate failure, you're 
sending an email and waiting days. That blocks development. That blocks QA. 
That slows every payment integration you build.

## What Mandas does

- Full ISO 20022 message support — pacs.008, pacs.004, pain.002, camt.054
- Triggerable R-transactions on demand — no email, one API call
- Stateful payment lifecycle simulation
- Runs locally via Docker — zero to running in under 5 minutes
- Programmable scenarios for CI/CD pipelines

## Repositories

| Repo | Description |
|---|---|
| [`mandas-core`](https://github.com/mandas-io/mandas-core) | Open source simulation engine (ISO 20022, SEPA, SWIFT) |
| [`mandas-docker`](https://github.com/mandas-io/mandas-docker) | Official Docker image and Compose setup |
| [`mandas-sdk`](https://github.com/mandas-io/mandas-sdk) | TypeScript and Python client SDKs |
| [`mandas-scenarios`](https://github.com/mandas-io/mandas-scenarios) | Community library of pre-built test scenarios |
| [`mandas-docs`](https://github.com/mandas-io/mandas-docs) | Documentation site source |

## Get started

```bash
docker pull mandasio/mandas-core
docker run -p 8080:8080 mandasio/mandas-core
```

Full documentation at [mandas.io](https://mandas.io)

---

*Simulate payments. Ship with confidence.*
