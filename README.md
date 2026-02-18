```mermaid
graph TD
    Start((**Початок**)) --> Audit[1. Енергоаудит та ТЕО]
    Audit --> Platform{2. Реєстрація в **Acivelex**}
    
    Platform --> Verification[3. Зелена Верифікація / ESG оцінка]
    
    Verification --> Funding{4. Вибір фінансування}
    
    Funding -->|Ринок| Bonds[Зелені Облігації]
    Funding -->|Банки| Loans[Пільгові кредити МФО]
    Funding -->|Держава| Grants[Гранти / Субвенції]
    
    Bonds --> Implement[5. Реалізація проекту]
    Loans --> Implement
    Grants --> Implement
    
    Implement --> Monitoring[6. Моніторинг та звітність]
    Monitoring --> End((**Успіх**))

    style Platform fill:#e1f5fe,stroke:#01579b,stroke-width:2px
    style Verification fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px
    style Funding fill:#fff3e0,stroke:#ef6c00,stroke-width:2px
