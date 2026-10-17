# Architecture

Draw it first on paper. Then transcribe here as a mermaid diagram.

```mermaid
flowchart LR
    client[Client] --> lb[Load balancer]
    lb --> api[Shortener API]
    api --> cache[(Cache)]
    cache -->|miss| db[(Datastore)]
    api --> idgen[ID generation]
```

## Components

| Component | Job | Why this and not the alternative |
|---|---|---|
| | | |

## Request paths

**Write (shorten a URL):**

**Read (follow a short link):**
