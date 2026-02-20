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
    Step2 --> Act2["Отримання погодження Мінфіну України"]

    %% Етап 3
    Act2 --> Step3["Етап 3. Розробка Зеленої рамки та Верифікація"]
    Law1["ст. 18 ЗУ Про ринки капіталу та організовані товарні ринки"]
    Step3 --- Law1
    Step3 --> Act3["Підтвердження екологічності проєкту:висновок SPO"]

    %% Етап 4
    Act3 --> Step4["Етап 4. Реєстрація випуску зелених облігацій"]
    Law4["Рішення НКЦПФР №391"]
    Step4 --- Law4
    Step4 --> Act4["Друге рішення ради: про емісію зелених облігацій"]
    Act4 --> Act5["Подання проспекту емісії до НКЦПФР"]
    Act5 --> Act6["Присвоєння номера ISIN в НДУ"]

    %% Етап 5
    Act6 --> Step5["Етап 5. Розміщення зелених облігацій та Щорічна звітність"]
    Law1["ст. 18 ЗУ Про ринки капіталу та організовані товарні ринки"]
    Step5 --- Law1
    Step5 --> Act7["Результат"]

    classDef mainNode fill:#f5f5f5,stroke:#333,stroke-width:4px,padding:50px 0px;
    classDef lawNode fill:#f9f9f9,stroke:#999,stroke-width:2px,stroke-dasharray: 1 1,padding:50px 0px;
    classDef actionNode fill:#fff,stroke:#333,stroke-width:3px,padding:50px 1px;
    classDef highlightNode fill:#fff3e0,stroke:#ef6c00,stroke-width:5px,padding:50px 0px;
    classDef successNode fill:#e8f5e9,stroke:#2e7d32,stroke-width:5px,padding:50px 0px;


    %% ЗАСТОСУВАННЯ КЛАСІВ
    class Step1,Step2,Step3,Step4,Step5 mainNode;
    class Law1,Law2,Law3,Law4,Law5 lawNode;
    class Act1,Act2,Act3,Act4,Act5,Act6 actionNode;
    class Act7 successNode;
