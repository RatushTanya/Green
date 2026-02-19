### Процедура випуску муніципальних зелених облігацій

```mermaid
graph TD
    %% Етап 1
    Step1["Етап 1. Стратегічне планування"]
    Law1["ст. 18 ЗУ Про ринки капіталу"]
    Step1 --- Law1
    Step1 --> Act1["Рішення ради про перелік проектів та СЕО"]

    %% Етап 2
    Act1 --> Step2["Етап 2. Бюджетне погодження"]
    Law2["ст. 74 Бюджетного кодексу"]
    Step2 --- Law2
    Step2 --> Act2["Отримання погодження Мінфіну"]

    %% Етап 3
    Act2 --> Step3["Етап 3. Розробка Framework та SPO"]
    Standard3["Стандарти ICMA / Верифікатор"]
    Step3 --- Standard3
    Step3 --> Act3["Отримання Second Party Opinion"]

    %% Етап 4
    Act3 --> Step4["Етап 4. Реєстрація та випуск"]
    Law4["Рішення НКЦПФР №391"]
    Step4 --- Law4
    Step4 --> Act4["Присвоєння ISIN у Депозитарії"]

    %% Етап 5
    Act4 --> Step5["Етап 5. Розміщення та звітність"]
    Step5 --> Act5["Аукціон та щорічний Impact Reporting"]

    %% Стилі
    style Step1 fill:#f5f5f5,stroke:#333
    style Step5 fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px
    style Law1 fill:#fff8e1,stroke:#ff8f00
    style Law2 fill:#fff8e1,stroke:#ff8f00
    style Law4 fill:#fff8e1,stroke:#ff8f00
