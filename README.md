### Юридична процедура отримання зелених інвестицій

```mermaid
graph TD
    %% Етап 1
    Step1["<b>Етап 1. Юридичне обґрунтування</b><br/>Відбір проєкту з еко-ефектом"]
    Law1["<i>ст. 18 ЗУ 'Про ринки капіталу'</i>"]
    
    Step1 --- Law1
    Step1 --> Decision{"Рішення міської ради<br/>про перелік проєктів"}

    %% Етап 2
    Decision --> Step2["<b>Етап 2. Бюджетне погодження</b><br/>Контроль лімітів боргу"]
    Law2["<i>ст. 74 Бюджетного кодексу<br/>Постанова КМУ №110</i>"]
    
    Step2 --- Law2
    Step2 --> MinFin["Погодження від<br/>Міністерства фінансів"]

    %% Етап 3
    MinFin --> Step3["<b>Етап 3. Green Bond Framework</b><br/>Розробка 'Зеленої рамки' та SPO"]
    Standard3["<i>Стандарти ICMA (GBP)<br/>Зовнішній верифікатор</i>"]
    
    Step3 --- Standard3
    Step3 --> Verified["Отримання Second Party<br/>Opinion (SPO)"]

    %% Етап 4
    Verified --> Step4["<b>Етап 4. Реєстрація в НКЦПФР</b><br/>Юридичне народження паперів"]
    Law4["<i>Рішення НКЦПФР №391</i>"]
    
    Step4 --- Law4
    Step4 --> Result(("<b>ISIN у Депозитарії</b><br/>Випуск активовано"))

    %% Стилізація
    style Step1 fill:#f9f9f9,stroke:#333
    style Step2 fill:#f9f9f9,stroke:#333
    style Step3 fill:#f9f9f9,stroke:#333
    style Step4 fill:#f9f9f9,stroke:#333
    style Result fill:#e1f5fe,stroke:#01579b,stroke-width:2px
    style Law1 fill:#fff3e0,stroke:#ef6c00,stroke-dasharray: 5 5
    style Law2 fill:#fff3e0,stroke:#ef6c00,stroke-dasharray: 5 5
    style Standard3 fill:#fff3e0,stroke:#ef6c00,stroke-dasharray: 5 5
    style Law4 fill:#fff3e0,stroke:#ef6c00,stroke-dasharray: 5 5
