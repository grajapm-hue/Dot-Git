# Mermaid Style Learning File

## 1. Basic Flowchart

```mermaid
flowchart LR
    A[Start] --> B[Process]
    B --> C[End]
```

---

## 2. Fill and Stroke Colors

```mermaid
flowchart LR
    A[Red Box]
    B[Green Box]
    C[Blue Box]

    A --> B --> C

    style A fill:#ffcccc,stroke:#ff0000,stroke-width:3px
    style B fill:#ccffcc,stroke:#00aa00,stroke-width:3px
    style C fill:#ccccff,stroke:#0000ff,stroke-width:3px
```

---

## 3. Dashed Connection

```mermaid
flowchart LR
    A --> B
    B -.-> C
    C --> D
```

---

## 4. Thick Connection

```mermaid
flowchart LR
    A ==> B
    B ==> C
```

---

## 5. Text on Arrow

```mermaid
flowchart LR
    A -->|Data| B
    B -->|Result| C
```

---

## 6. Bidirectional Arrow

```mermaid
flowchart LR
    A <--> B
```

---

## 7. Different Node Shapes

```mermaid
flowchart LR
    A[Rectangle]
    B(Rounded)
    C((Circle))
    D{Decision}
    E>Flag]
```

---

## 8. Subgraph Example

```mermaid
flowchart LR

subgraph Input
    A[Sensor]
    B[Switch]
end

subgraph Processing
    C[Arduino]
end

subgraph Output
    D[LCD]
    E[Buzzer]
end

A --> C
B --> C
C --> D
C --> E
```

---

## 9. Class Definitions

```mermaid
flowchart LR

A[Input]
B[Controller]
C[Output]

A --> B --> C

classDef red fill:#ffcccc,stroke:#ff0000,stroke-width:2px;
classDef green fill:#ccffcc,stroke:#00aa00,stroke-width:2px;
classDef blue fill:#ccccff,stroke:#0000ff,stroke-width:2px;

class A red;
class B green;
class C blue;
```

---

## 10. Dashed Border Node

```mermaid
flowchart LR

A[Normal]
B[Dashed Border]

A --> B

style B fill:#ffffcc,stroke:#000000,stroke-width:2px,stroke-dasharray: 5 5
```

---

## 11. Multiple Arrow Types

```mermaid
flowchart LR

A --> B
B -.-> C
C ==> D
D --> E
```

---

## 12. Sequence Diagram

```mermaid
sequenceDiagram

User->>Server: Request
Server->>Database: Query
Database-->>Server: Result
Server-->>User: Response
```

---

## 13. State Diagram

```mermaid
stateDiagram-v2

[*] --> Idle
Idle --> Running
Running --> Stopped
Stopped --> [*]
```

---

## 14. Gantt Chart

```mermaid
gantt
title Project Plan

section Design
Requirement :done, a1, 2026-01-01, 5d
Design :a2, after a1, 7d

section Coding
Development :a3, after a2, 10d
Testing :a4, after a3, 5d
```

---

## 15. Pie Chart

```mermaid
pie title Energy Usage

"AC" : 40
"Lights" : 20
"Fans" : 15
"TV" : 10
"Others" : 15
```

---

## 16. Arduino Energy Monitor Example

```mermaid
flowchart LR

M[Energy Meter]
S[Current Sensor]
A[Arduino UNO]
L[LCD Display]
G[GSM Module]
P[Mobile Phone]

M --> S
S --> A
A --> L
A --> G
G --> P

style M fill:#ffd6d6,stroke:#ff0000,stroke-width:2px
style S fill:#fff2cc,stroke:#ffaa00,stroke-width:2px
style A fill:#d9ead3,stroke:#00aa00,stroke-width:3px
style L fill:#cfe2f3,stroke:#0000ff,stroke-width:2px
style G fill:#ead1dc,stroke:#990099,stroke-width:2px
style P fill:#f4cccc,stroke:#cc0000,stroke-width:2px
```

---

## 17. Dark Theme

```mermaid
%%{init: {
'theme':'dark'
}}%%

flowchart LR

A --> B --> C
```

---

## 18. Forest Theme

```mermaid
%%{init: {
'theme':'forest'
}}%%

flowchart LR

A --> B --> C
```

---

## 19. Neutral Theme

```mermaid
%%{init: {
'theme':'neutral'
}}%%

flowchart LR

A --> B --> C
```

---

## 20. Large Combined Demo

```mermaid
flowchart TD

A([START])

B{Power ON?}

C[Initialize System]

D[Read Sensor]

E{Threshold Exceeded?}

F[Send SMS]

G[Update LCD]

H([END])

A --> B

B -->|YES| C

B -->|NO| H

C --> D

D --> E

E -->|YES| F

E -->|NO| G

F --> G

G --> D

style A fill:#d5f5e3,stroke:#28b463,stroke-width:3px
style H fill:#fadbd8,stroke:#cb4335,stroke-width:3px
style E fill:#fcf3cf,stroke:#d4ac0d,stroke-width:2px
style F fill:#ebdef0,stroke:#8e44ad,stroke-width:2px
```