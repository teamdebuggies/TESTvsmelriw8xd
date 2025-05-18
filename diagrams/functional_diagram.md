graph TD
    A[User Interface] -->|Review Asset Portfolios| B[Portfolio Service]
    A -->|Register Transactions| C[Transaction Service]
    A -->|Download Reports| D[Reporting Service]
    E[Internal Staff Interface] -->|Execute Transactions| C
    E -->|Update Asset Info| B
    E -->|Manage Reports| D
    B -->|Read/Write| F[Asset Database]
    C -->|Read/Write| F
    D -->|Read| F
    F -->|Queries| G[Oracle DB]