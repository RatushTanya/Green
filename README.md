graph LR
    %% Зміна напрямку на LR (Left to Right) робить схему горизонтальною

    %% Етап 1
    Step1["<h4>Етап 1. Стратегічне планування</h4>"]
    Law1_1["ст. 18 ЗУ Про ринки капіталу"]
    Step1 --- Law1_1
    Step1 --> Act1["Перше рішення міської ради про емісію"]

    %% Етап 2
    Act1 --> Step2["<h4>Етап 2. Бюджетне погодження</h4>"]
    Law2["ст. 74 Бюджетного кодексу"]
    Law3["Постанова КМУ №110"]
    Step2 --- Law3
    Law3 --- Law2
    Step2 --> Act2["Отримання погодження Мінфіну"]

    %% Етап 3
    Act2 --> Step3["<h4>Етап 3. Розробка Зеленої рамки</h4>"]
    Step3 --> Act3["Розробка Зеленої рамки за стандартами ICMA"]

    %% Етап 4
    Act3 --> Step4["<h4>Етап 4. Верифікація</h4>"]
    Law1_2["ст. 18 ЗУ Про ринки капіталу"]
    Step4 --- Law1_2
    Step4 --> Act4["Підтвердження екологічності проєкту (SPO)"]

    %% Етап 5
    Act4 --> Step5["<h4>Етап 5. Реєстрація випуску</h4>"]
    Law4["Рішення НКЦПФР №391"]
    Step5 --- Law4
    Step5 --> Act5["Друге рішення міської ради"]
    Act5 --> Act6["Подання проспекту до НКЦПФР <br/> та присвоєння ISIN"]
    
    %% Етап 6
    Act6 --> Step6["<h4>Етап 6. Розміщення та звітність</h4>"]
    Law1_3["ст. 18 ЗУ Про ринки капіталу"]
    Step6 --- Law1_3
    Step6 --> Act7["Старт проєкту та <br/>щорічний Impact Reporting"]

    %% СТИЛІЗАЦІЯ
    %% Використовуємо #E1F5FE для світло-блакитного (правове поле)
    classDef mainNode fill:#f5f5f5,stroke:#333,stroke-width:2px;
    classDef lawNode fill:#E1F5FE,stroke:#01579b,stroke-width:1px,stroke-dasharray: 5 5;
    classDef actionNode fill:#fff,stroke:#333,stroke-width:2px;
    classDef successNode fill:#e8f5e9,stroke:#2e7d32,stroke-width:3px;

    %% ЗАСТОСУВАННЯ КЛАСІВ
    class Step1,Step2,Step3,Step4,Step5,Step6 mainNode;
    class Law1_1,Law1_2,Law1_3,Law2,Law3,Law4 lawNode;
    class Act1,Act2,Act3,Act4,Act5,Act6 actionNode;
    class Act7 successNode;
