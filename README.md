```mermaid
%%{init: {'flowchart': {'nodeSpacing': 10, 'rankSpacing': 15}}}%%
graph TD

    %% Етап 1
    Step1["<h4>Етап 1. Стратегічне планування</h4>"]
    Law1_1["ст.18 ЗУ Про ринки капіталу"]
    Step1 --- Law1_1 & Act1["Перше рішення ради про емісію"]

    %% Етап 2
    Act1 --> Step2["<h4>Етап 2. Бюджетне погодження</h4>"]
    Law2["ст.74 БК України"]
    Law3["ПКМУ №110"]
    Step2 --- Law2 --- Law3
    Step2 --> Act2["Отримання погодження Мінфіну"]

    %% Етап 3
    Act2 --> Step3["<h4>Етап 3. Розробка Зеленої рамки</h4>"]
    Step3 --> Act3["Framework за стандартами ICMA"]

    %% Етап 4
    Act3 --> Step4["<h4>Етап 4. Верифікація</h4>"]
    Law1_2["ст.18 ЗУ Про ринки капіталу"]
    Step4 --- Law1_2 & Act4["Підтвердження екологічності"]

    %% Етап 5
    Act4 --> Step5["<h4>Етап 5. Реєстрація випуску</h4>"]
    Law4["Рішення НКЦПФР №391"]
    Step5 --- Law4
    Step5 --> Act5["Друге рішення міської ради"]
    Act5 --> Act6["Проспект НКЦПФР та ISIN"]
    
    %% Етап 6
    Act6 --> Step6["<h4>Етап 6. Розміщення та звітність</h4>"]
    Law1_3["ст.18 ЗУ Про ринки капіталу"]
    Step6 --- Law1_3 & Act7["Старт та Impact Reporting"]

    %% СТИЛІЗАЦІЯ (Компактна)
    classDef mainNode fill:#f5f5f5,stroke:#333,stroke-width:2px,padding:5px;
    classDef lawNode fill:#E1F5FE,stroke:#01579b,stroke-width:1px,stroke-dasharray: 3 3,padding:2px;
    classDef actionNode fill:#fff,stroke:#333,stroke-width:2px,padding:5px;
    classDef successNode fill:#e8f5e9,stroke:#2e7d32,stroke-width:3px,padding:10px;

    %% ЗАСТОСУВАННЯ КЛАСІВ
    class Step1,Step2,Step3,Step4,Step5,Step6 mainNode;
    class Law1_1,Law1_2,Law1_3,Law2,Law3,Law4 lawNode;
    class Act1,Act2,Act3,Act4,Act5,Act6 actionNode;
    class Act7 successNode;
