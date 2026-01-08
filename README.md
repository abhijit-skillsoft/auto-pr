flowchart LR
    subgraph planMode [Cursor Plan Mode]
        P1[Phase 1: Planning] --> P2[Phase 2: Execution]
    end
    
    subgraph phase1 [Planning Phase]
        A[Analyze Requirements] --> B[Review Codebase]
        B --> C[Propose Architecture]
        C --> D[Human Approval]
    end
    
    subgraph phase2 [Execution Phase]
        E[Generate Code] --> F[Run Validation]
        F --> G[Iterate on Feedback]
    end
    
    P1 -.-> phase1
    P2 -.-> phase2
