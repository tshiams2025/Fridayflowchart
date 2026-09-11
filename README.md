```mermaid # Fridayflowchart

graph TD
    %% Styling Definitions
    classDef header fill:#A3E635,stroke:#333,stroke-width:2px,font-weight:bold;
    classDef mainJob fill:#E5E7EB,stroke:#333,stroke-width:1px;
    classDef applyJob fill:#6B21A8,color:#fff,stroke:#333,stroke-width:1px,font-weight:bold;

    %% Header Row
    H1[JOB]:::header --> H2[APPLY JOB]:::header

    %% Section 1: Home & House Chores
    subgraph House Chores
        Job1[Home / Programm / Self-]:::mainJob
        App1_1[House]:::applyJob
        App1_2[Cook all week]:::applyJob
        App1_3[Wash the dishes]:::applyJob
        
        Job1 --> App1_1
        Job1 --> App1_2
        Job1 --> App1_3
    end

    %% Section 2: Video Games
    subgraph Gaming
        Job2[Gaming]:::mainJob
        App2_1[Play video games]:::applyJob
        
        Job2 --> App2_1
    end

    %% Section 3: Marketing
    subgraph Business
        Job3[Business / Project]:::mainJob
        App3_1[Hire a marketing Company]:::applyJob
        
        Job3 --> App3_1
    end

    %% Section 4: Automation
    subgraph Automation
        Job4[Build n8n]:::header
    end

    %% Connecting sections for flow structure
    H2 --> Job1
    Job1 --> Job2
    Job2 --> Job3
    Job3 --> Job4 ```
