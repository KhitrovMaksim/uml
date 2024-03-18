# UML

## Sequence

```mermaid
sequenceDiagram
    Alice->>John: Hello John, how are you?
    loop HealthCheck
        John->>John: Fight against hypochondria
    end
    Note right of John: Rational thoughts!
    John-->>Alice: Great!
    John->>Bob: How about you?
    Bob-->>John: Jolly good!
```

```mermaid
sequenceDiagram
    actor Consumer
    participant API
    database DB
    Consumer->>api: { email, password }
    API-->>DB: { email }
    DB-->>API: { user: { id, email, name, hash } }
    API-->>API: check hash
    API-->>Consumer: { user: { id, email, name } }
```
```mermaid
sequenceDiagram
    actor A as Alice
    database J as John
    A->>J: Hello John, how are you?
    J->>A: Great!
```
## Flowchart

```mermaid
flowchart LR

A[Hard] -->|Text| B(Round)
B --> C{Decision}
C -->|One| D[Result 1]
C -->|Two| E[Result 2]
```
