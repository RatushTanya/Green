```mermaid
graph TD
    %% Етап 1
    Step1["<h4>Етап 1. Стратегічне планування</h4>"]
    Law1["ст. 18 ЗУ Про ринки капіталу"]
    Step1 --- Law1
    Step1 --> Act1["Перше рішення міської ради про емісію"]

    %% Етап 2
    Act1 --> Step2["<h4>Етап 2. Бюджетне погодження</h4>"]
    Law2["ст. 74 Бюджетного кодексу"]
    Law3["Постанова КМУ №110"]
    Step2 --- Law2 ---Law3
    Step2 --> Act2["Отримання погодження Мінфіну"]

    %% Етап 3
    Act2-->Step3["<h4>Етап 3. Розробка Зеленої рамки</h4>"]
    Step3 --> Act3["Розробка Зеленої рамки за стандартами ICMA"]

    %% Етап 4
    Act3 --> Step4["<h4>Етап 4. Верифікація</h4>"]
    Law1["ст. 18 ЗУ Про ринки капіталу"]
    Step4 --- Law1
    Step4 --> Act4["Підтвердження екологічності проєкту"]

    %% Етап 5
    Act4 --> Step5["<h4>Етап 5. Реєстрація випуску зелених облігацій</h4>"]
    Law4["Рішення НКЦПФР №391"]
    Step5 --- Law4
    Step5 --> Act5["Друге рішення міської ради про емісію"]
    Act5 --> Act6["Подання проспекту емісії до НКЦПФР та Присвоєння номера ISIN"]
    
    %% Етап 6
    Act6 --> Step6["<h4>Етап 6. Розміщення зелених облігацій та Щорічна звітність</h4>"]
    Law1["ст. 18 ЗУ Про ринки капіталу"]
    Step6 --- Law1
    Step6 --> Act7["Результат"]

    classDef mainNode fill:#f5f5f5,stroke:#333,stroke-width:4px,padding:100px 0px;
    classDef lawNode fill:#f9f9f9,stroke:#999,stroke-width:2px,stroke-dasharray: 1 1,padding:100px 0px;
    classDef actionNode fill:#fff,stroke:#333,stroke-width:3px,padding:100px 0px;
    classDef highlightNode fill:#fff3e0,stroke:#ef6c00,stroke-width:5px,padding:100px 0px;
    classDef successNode fill:#e8f5e9,stroke:#2e7d32,stroke-width:5px,padding:100px 0px;


    %% ЗАСТОСУВАННЯ КЛАСІВ
    class Step1,Step2,Step3,Step4,Step5,Step6 mainNode;
    class Law1,Law2,Law3,Law4 lawNode;
    class Act1,Act2,Act3,Act4,Act5,Act6 actionNode;
    class Act7 successNode;
