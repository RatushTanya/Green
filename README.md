```mermaid
graph TD
    %% Налаштування відступів для зміни висоти/ширини вузлів
    %% Використовуємо великий горизонтальний padding і малий вертикальний
    
    Step1["Етап 1. Стратегічне планування"]
    Law1["ст. 18 ЗУ Про ринки капіталу"]
    Step1 --- Law1
    Step1 --> Act1["Перше рішення ради: перелік проєктів та СЕО"]

    Act1 --> Step2["Етап 2. Бюджетне погодження"]
    Law2["ст. 74 Бюджетного кодексу"]
    Step2 --- Law2
    Step2 --> Act2["Отримання висновку Мінфіну України"]

    Act2 --> Step3["Етап 3. Framework та Верифікація"]
    Standard3["Принципи ICMA / Висновок SPO"]
    Step3 --- Standard3
    Step3 --> Act3["Підтвердження екологічності проєкту"]

    Act3 --> Step4["Етап 4. Реєстрація випуску"]
    Law4["Рішення НКЦПФР №391"]
    Step4 --- Law4
    Step4 --> CouncilFinal["Друге рішення ради: про запозичення"]
    CouncilFinal --> Act4["Подання проспекту емісії до НКЦПФР"]
    Act4 --> ISIN["Присвоєння номера ISIN в НДУ"]

    ISIN --> Step5["Етап 5. Розміщення та звітність"]
    Law5["ст. 18 ЗУ Про ринки капіталу"]
    Step5 --- Law5
    Step5 --> Act5["Продаж облігацій та Impact Reporting"]

    %% СТИЛІЗАЦІЯ: товсті рамки (stroke-width:4px)
    classDef thickStep fill:#f5f5f5,stroke:#333,stroke-width:4px,padding:20px 5px;
    classDef thickLaw fill:#f9f9f9,stroke:#999,stroke-width:2px,stroke-dasharray: 5 5;
    classDef thickAction fill:#fff,stroke:#333,stroke-width:3px;
    classDef specialNode fill:#fff3e0,stroke:#ef6c00,stroke-width:5px;
    classDef greenNode fill:#e8f5e9,stroke:#2e7d32,stroke-width:5px;

    %% Призначення класів
    class Step1,Step2,Step3,Step4 thickStep;
    class Law1,Law2,Law4,Law5 thickLaw;
    class Act1,Act2,Act3,Act4,ISIN,Act5 thickAction;
    class CouncilFinal specialNode;
    class Step5 greenNode;
