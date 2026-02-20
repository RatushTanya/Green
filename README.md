```mermaid
graph TD
    %% Етап 1
    Step1["Етап 1. Стратегічне планування"]
    Law1["ст. 18 ЗУ Про ринки капіталу та організовані товарні ринки"]
    Step1 --- Law1
    Step1 --> Act1["Перше рішення ради: про емісію облігацій"]

    %% Етап 2
    Act1 --> Step2["Етап 2. Бюджетне погодження"]
    Law2["ст. 74 Бюджетного кодексу України"]
    Law3["Постанова КМУ №110"]
    Step2 --- Law2
    Step2 --- Law3
    Step2 --> Act2["Отримання висновку Мінфіну України"]

    %% Етап 3
    Act2 --> Step3["Етап 3. Framework та Верифікація"]
    Standard3["Принципи ICMA / Висновок SPO"]
    Step3 --- Standard3
    Step3 --> Act3["Підтвердження екологічності проєкту"]

    %% Етап 4
    Act3 --> Step4["Етап 4. Реєстрація випуску"]
    Law4["Рішення НКЦПФР №391"]
    Step4 --- Law4
    Step4 --> CouncilFinal["Друге рішення ради: про здійснення запозичення"]
    CouncilFinal --> Act4["Подання проспекту емісії до НКЦПФР"]
    Act4 --> ISIN["Присвоєння номера ISIN в НДУ"]

    %% Етап 5
    ISIN --> Step5["Етап 5. Розміщення та звітність"]
    Law5["ст. 18 ЗУ Про ринки капіталу"]
    Step5 --- Law5
    Step5 --> Act5["Продаж облігацій та щорічний Impact Reporting"]

    %% Стилі (кольори)
    style Step1 fill:#f5f5f5,stroke:#333
    style CouncilFinal fill:#fff3e0,stroke:#ef6c00,stroke-width:2px
    style Step5 fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px
    style Law1 fill:#f9f9f9,stroke:#999,stroke-dasharray: 5 5
    style Law2 fill:#f9f9f9,stroke:#999,stroke-dasharray: 5 5
    style Law3 fill:#f9f9f9,stroke:#999,stroke-dasharray: 5 5
    style Law4 fill:#f9f9f9,stroke:#999,stroke-dasharray: 5 5
    style Law5 fill:#f9f9f9,stroke:#999,stroke-dasharray: 5 5
