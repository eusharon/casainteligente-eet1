<!DOCTYPE html>
<html lang="pt-BR">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Casa Inteligente | EET1 - CIAA</title>

    <style>

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background: #06111f;
            color: #eef7ff;
            line-height: 1.7;
        }

        /* =========================
           MENU
        ========================= */

        nav {
            position: sticky;
            top: 0;
            z-index: 1000;

            background: rgba(3, 11, 20, 0.94);

            backdrop-filter: blur(12px);

            border-bottom: 1px solid #1c354c;
        }

        .nav-container {
            max-width: 1150px;
            margin: auto;

            padding: 17px 25px;

            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .logo {
            font-weight: bold;
            letter-spacing: 1px;
        }

        .logo span {
            color: #20d8ff;
        }

        .menu a {
            color: #b8c9da;
            text-decoration: none;
            margin-left: 22px;
            font-size: 14px;

            transition: 0.3s;
        }

        .menu a:hover {
            color: #20d8ff;
        }

        /* =========================
           HERO
        ========================= */

        .hero {

            min-height: 85vh;

            display: flex;
            align-items: center;

            padding: 80px 6%;

            background:
                linear-gradient(
                    rgba(3, 12, 24, 0.88),
                    rgba(3, 12, 24, 0.96)
                ),
                url("casa-inteligente-1.jpg");

            background-size: cover;
            background-position: center;
        }

        .hero-content {
            max-width: 1150px;
            width: 100%;
            margin: auto;
        }

        .tag {

            display: inline-block;

            padding: 8px 16px;

            border-radius: 30px;

            border: 1px solid #20d8ff;

            color: #4ce1ff;

            font-size: 13px;

            font-weight: bold;

            letter-spacing: 1px;
        }

        .hero h1 {

            font-size: clamp(3rem, 8vw, 6.5rem);

            line-height: 0.95;

            margin: 25px 0;
        }

        .hero h1 span {
            color: #20d8ff;
        }

        .hero p {

            max-width: 750px;

            color: #b9c9d9;

            font-size: 1.15rem;
        }

        .button {

            display: inline-block;

            margin-top: 30px;

            padding: 13px 22px;

            background: #20d8ff;

            color: #00121d;

            text-decoration: none;

            font-weight: bold;

            border-radius: 10px;

            transition: 0.3s;
        }

        .button:hover {

            transform: translateY(-3px);

            box-shadow: 0 10px 30px rgba(32, 216, 255, 0.25);
        }

        /* =========================
           SEÇÕES
        ========================= */

        section {
            padding: 90px 6%;
        }

        .container {
            max-width: 1150px;
            margin: auto;
        }

        .section-label {

            color: #20d8ff;

            font-size: 13px;

            font-weight: bold;

            text-transform: uppercase;

            letter-spacing: 2px;
        }

        .section-title {

            font-size: clamp(2rem, 5vw, 3.5rem);

            margin: 5px 0 15px;
        }

        .section-description {

            color: #9eb1c5;

            max-width: 800px;
        }

        .dark-section {
            background: #081522;
        }

        /* =========================
           IMAGENS
        ========================= */

        .image-box {

            margin-top: 40px;

            border-radius: 20px;

            overflow: hidden;

            border: 1px solid #23435c;

            box-shadow: 0 20px 60px rgba(0,0,0,0.3);
        }

        .image-box img {

            width: 100%;

            display: block;
        }

        .image-caption {

            padding: 15px 20px;

            background: #0b1c2d;

            color: #9eb1c5;

            font-size: 14px;
        }

        /* =========================
           CARDS
        ========================= */

        .cards {

            display: grid;

            grid-template-columns:
                repeat(3, 1fr);

            gap: 20px;

            margin-top: 40px;
        }

        .card {

            background:
                linear-gradient(
                    145deg,
                    #0d2033,
                    #081523
                );

            border: 1px solid #1d3a53;

            border-radius: 17px;

            padding: 28px;

            transition: 0.3s;
        }

        .card:hover {

            transform: translateY(-6px);

            border-color: #20d8ff;

            box-shadow:
                0 15px 40px rgba(0, 200, 255, 0.08);
        }

        .card-icon {

            font-size: 32px;

            margin-bottom: 12px;
        }

        .card h3 {
            margin-bottom: 8px;
        }

        .card p {
            color: #9eb1c5;
            font-size: 15px;
        }

        /* =========================
           FLUXO
        ========================= */

        .flow {

            display: grid;

            grid-template-columns:
                repeat(4, 1fr);

            gap: 15px;

            margin-top: 40px;
        }

        .flow-card {

            text-align: center;

            background: #091b2b;

            border: 1px solid #21415b;

            border-radius: 15px;

            padding: 25px 15px;
        }

        .flow-card .number {

            width: 45px;
            height: 45px;

            margin: auto;

            display: flex;

            align-items: center;
            justify-content: center;

            border-radius: 50%;

            background: rgba(32,216,255,0.1);

            color: #20d8ff;

            font-weight: bold;

            font-size: 20px;
        }

        .flow-card h3 {
            margin: 12px 0 5px;
        }

        .flow-card p {
            color: #91a6bb;
            font-size: 14px;
        }

        /* =========================
           EXPLICAÇÃO
        ========================= */

        .explanation {

            display: grid;

            grid-template-columns:
                1fr 1fr;

            gap: 45px;

            align-items: center;

            margin-top: 45px;
        }

        .explanation img {

            width: 100%;

            border-radius: 18px;

            border: 1px solid #24435b;
        }

        .explanation p {

            color: #a8bacd;

            margin-bottom: 17px;
        }

        .highlight {

            padding: 18px 20px;

            border-left: 3px solid #20d8ff;

            background: rgba(32,216,255,0.05);

            color: #dcecf7;

            margin-top: 20px;
        }

        /* =========================
           COMPONENTES
        ========================= */

        .components {

            display: grid;

            grid-template-columns:
                repeat(2, 1fr);

            gap: 18px;

            margin-top: 40px;
        }

        .component {

            padding: 23px;

            background: #0a1b2b;

            border-left: 3px solid #20d8ff;

            border-radius: 8px;
        }

        .component h3 {
            margin-bottom: 5px;
        }

        .component p {
            color: #9db0c4;
        }

        /* =========================
           EQUIPE
        ========================= */

        .team-section {

            background:
                linear-gradient(
                    135deg,
                    #071c2e,
                    #06101c
                );

            text-align: center;
        }

        .team-box {

            max-width: 950px;

            margin: 40px auto 0;

            padding: 45px 30px;

            background: rgba(12, 33, 50, 0.7);

            border: 1px solid #28516b;

            border-radius: 22px;
        }

        .team-box p {

            max-width: 850px;

            margin: 15px auto;

            color: #b4c5d6;
        }

        .names {

            display: flex;

            justify-content: center;

            flex-wrap: wrap;

            gap: 10px;

            margin-top: 30px;
        }

        .name {

            padding: 8px 14px;

            background: #0b2032;

            border: 1px solid #29465d;

            border-radius: 30px;

            font-size: 14px;
        }

        /* =========================
           FOOTER
        ========================= */

        footer {

            padding: 35px 20px;

            text-align: center;

            background: #030a12;

            color: #71869a;
        }

        footer strong {
            color: #e3f2ff;
        }

        /* =========================
           RESPONSIVIDADE
        ========================= */

        @media (max-width: 850px) {

            .menu {
                display: none;
            }

            .cards {
                grid-template-columns: 1fr 1fr;
            }

            .flow {
                grid-template-columns: 1fr 1fr;
            }

            .explanation {
                grid-template-columns: 1fr;
            }

        }

        @media (max-width: 600px) {

            section {
                padding: 65px 5%;
            }

            .cards,
            .components,
            .flow {
                grid-template-columns: 1fr;
            }

            .hero {
                min-height: 75vh;
            }

        }

    </style>

</head>


<body>


<!-- =========================
     MENU
========================= -->

<nav>

    <div class="nav-container">

        <div class="logo">
            EET1 <span>• CASA INTELIGENTE</span>
        </div>

        <div class="menu">

            <a href="#conceito">
                Conceito
            </a>

            <a href="#funcionamento">
                Funcionamento
            </a>

            <a href="#componentes">
                Componentes
            </a>

            <a href="#tecnologias">
                Tecnologias
            </a>

            <a href="#equipe">
                Equipe
            </a>

        </div>

    </div>

</nav>


<!-- =========================
     CAPA
========================= -->

<header class="hero">

    <div class="hero-content">

        <span class="tag">
            PROJETO PRÁTICO • CIAA
        </span>

        <h1>
            Casa<br>
            <span>Inteligente</span>
        </h1>

        <p>

            Uma maquete desenvolvida pela turma EET1
            para demonstrar, na prática, como a eletrônica,
            a programação e a automação podem trabalhar
            juntas para criar uma residência inteligente.

        </p>

        <a
            href="#conceito"
            class="button"
        >
            Conhecer o projeto ↓
        </a>

    </div>

</header>


<!-- =========================
     CONCEITO
========================= -->

<section id="conceito">

    <div class="container">

        <span class="section-label">
            01 • Conceito
        </span>

        <h2 class="section-title">
            O que é uma Casa Inteligente?
        </h2>

        <p class="section-description">

            Uma casa inteligente é uma residência que utiliza
            sensores, equipamentos eletrônicos e sistemas de
            controle para realizar tarefas automaticamente
            ou receber comandos do usuário.

        </p>


        <div class="image-box">

            <img
                src="casa-inteligente-1.jpg"
                alt="Maquete da Casa Inteligente"
            >

            <div class="image-caption">

                Visão geral da proposta da Casa Inteligente,
                desenvolvida pela turma EET1.

            </div>

        </div>


        <div class="cards">


            <div class="card">

                <div class="card-icon">
                    📡
                </div>

                <h3>
                    Sensores
                </h3>

                <p>

                    São responsáveis por perceber o ambiente.
                    Eles podem detectar presença, fumaça,
                    nível de água e outras condições.

                </p>

            </div>


            <div class="card">

                <div class="card-icon">
                    🧠
                </div>

                <h3>
                    Controle
                </h3>

                <p>

                    O Arduino recebe as informações dos sensores
                    e executa as regras definidas no programa.

                </p>

            </div>


            <div class="card">

                <div class="card-icon">
                    ⚡
                </div>

                <h3>
                    Atuadores
                </h3>

                <p>

                    São os componentes que realizam a ação,
                    como acender uma lâmpada, ligar uma bomba
                    ou emitir um alerta.

                </p>

            </div>


        </div>

    </div>

</section>


<!-- =========================
     AUTOMAÇÃO
========================= -->

<section class="dark-section">

    <div class="container">

        <span class="section-label">
            02 • Automação
        </span>

        <h2 class="section-title">
            O que é Automação?
        </h2>

        <p class="section-description">

            Automação é utilizar sistemas capazes de realizar
            determinadas tarefas automaticamente, seguindo
            regras previamente programadas.

        </p>


        <div class="highlight">

            <strong>
                De forma simples:
            </strong>

            o sistema percebe alguma coisa através de um sensor,
            o Arduino interpreta essa informação e depois
            determina qual ação deve acontecer.

        </div>


        <div class="flow">


            <div class="flow-card">

                <div class="number">
                    1
                </div>

                <h3>
                    Sensor
                </h3>

                <p>
                    Percebe uma situação.
                </p>

            </div>


            <div class="flow-card">

                <div class="number">
                    2
                </div>

                <h3>
                    Arduino
                </h3>

                <p>
                    Recebe e interpreta a informação.
                </p>

            </div>


            <div class="flow-card">

                <div class="number">
                    3
                </div>

                <h3>
                    Relé
                </h3>

                <p>
                    Realiza o acionamento.
                </p>

            </div>


            <div class="flow-card">

                <div class="number">
                    4
                </div>

                <h3>
                    Atuador
                </h3>

                <p>
                    Executa a ação.
                </p>

            </div>


        </div>

    </div>

</section>


<!-- =========================
     FUNCIONAMENTO
========================= -->

<section id="funcionamento">

    <div class="container">

        <span class="section-label">
            03 • Funcionamento
        </span>

        <h2 class="section-title">
            Como funciona a nossa maquete?
        </h2>

        <p class="section-description">

            A maquete reúne diversos componentes eletrônicos
            que trabalham em conjunto. Cada sensor fornece
            informações ao sistema e o Arduino decide como
            responder a elas.

        </p>


        <div class="image-box">

            <img
                src="casa-inteligente-2.jpg"
                alt="Diagrama do funcionamento da Casa Inteligente"
            >

            <div class="image-caption">

                Representação da arquitetura do projeto:
                sensores, Arduino Mega, relés, Bluetooth
                e dispositivos controlados.

            </div>

        </div>


        <div class="explanation">


            <div>

                <h2>
                    🧠 O Arduino é o cérebro do sistema
                </h2>

                <br>

                <p>

                    O Arduino Mega 2560 é utilizado como
                    unidade de controle da maquete.

                </p>

                <p>

                    Ele recebe informações provenientes
                    dos sensores e executa o programa
                    desenvolvido para o projeto.

                </p>

                <p>

                    O programa contém regras que dizem
                    ao Arduino o que fazer diante de
                    cada situação.

                </p>


                <div class="highlight">

                    <strong>
                        Exemplo:
                    </strong>

                    se o sensor detectar presença,
                    o programa pode mandar o sistema
                    acender uma iluminação.

                </div>

            </div>


            <div>

                <img
                    src="casa-inteligente-2.jpg"
                    alt="Arduino e sistema da maquete"
                >

            </div>


        </div>

    </div>

</section>


<!-- =========================
     COMPONENTES
========================= -->

<section
    class="dark-section"
    id="componentes"
>

    <div class="container">

        <span class="section-label">
            04 • Componentes
        </span>

        <h2 class="section-title">
            Principais componentes
        </h2>

        <p class="section-description">

            Cada componente possui uma função específica
            dentro do sistema.

        </p>


        <div class="components">


            <div class="component">

                <h3>
                    📡 Sensor de Presença
                </h3>

                <p>

                    Detecta movimento no ambiente.
                    Pode ser utilizado para acionar
                    automaticamente a iluminação.

                </p>

            </div>


            <div class="component">

                <h3>
                    🔥 Sensor de Fumaça
                </h3>

                <p>

                    Detecta a presença de fumaça e pode
                    enviar uma informação para o Arduino,
                    permitindo gerar um alerta.

                </p>

            </div>


            <div class="component">

                <h3>
                    💧 Sensor de Nível
                </h3>

                <p>

                    Verifica o nível da água na caixa
                    e permite que o sistema saiba
                    quando determinada condição foi atingida.

                </p>

            </div>


            <div class="component">

                <h3>
                    ⚙️ Sistema de Bombeamento
                </h3>

                <p>

                    Representa o funcionamento de uma bomba
                    utilizada para movimentar a água
                    dentro do sistema.

                </p>

            </div>


            <div class="component">

                <h3>
                    💡 Iluminação
                </h3>

                <p>

                    Representa equipamentos que podem
                    ser acionados automaticamente pelo sistema.

                </p>

            </div>


            <div class="component">

                <h3>
                    🔌 Módulo de Relés
                </h3>

                <p>

                    Permite que o Arduino controle
                    dispositivos elétricos através
                    de comandos de acionamento.

                </p>

            </div>


            <div class="component">

                <h3>
                    📱 Bluetooth HC-05
                </h3>

                <p>

                    Permite comunicação sem fio,
                    possibilitando enviar comandos
                    para o sistema através de um dispositivo compatível.

                </p>

            </div>


            <div class="component">

                <h3>
                    🛢️ Caixa d'Água
                </h3>

                <p>

                    Representa o armazenamento de água
                    e possui monitoramento de nível
                    dentro da proposta da maquete.

                </p>

            </div>


        </div>

    </div>

</section>


<!-- =========================
     TECNOLOGIAS
========================= -->

<section id="tecnologias">

    <div class="container">

        <span class="section-label">
            05 • Tecnologia
        </span>

        <h2 class="section-title">
            Arduino e SimulIDE
        </h2>

        <p class="section-description">

            O projeto une eletrônica, programação e simulação
            para transformar conceitos teóricos em uma aplicação prática.

        </p>


        <div class="explanation">


            <div>

                <h2>
                    🧠 Arduino Mega 2560
                </h2>

                <br>

                <p>

                    O Arduino Mega 2560 é uma placa baseada
                    em microcontrolador utilizada para controlar
                    os diferentes elementos do projeto.

                </p>

                <p>

                    Ele possui diversas entradas e saídas,
                    permitindo conectar sensores, LEDs,
                    módulos de relés, motores e outros componentes.

                </p>

                <p>

                    O programa gravado no Arduino determina
                    como ele deve reagir às informações recebidas.

                </p>

            </div>


            <div class="image-box">

                <img
                    src="casa-inteligente-2.jpg"
                    alt="Sistema baseado em Arduino"
                >

            </div>


        </div>


        <div class="explanation">


            <div class="image-box">

                <img
                    src="casa-inteligente-1.jpg"
                    alt="Projeto de Casa Inteligente"
                >

            </div>


            <div>

                <h2>
                    🖥️ SimulIDE
                </h2>

                <br>

                <p>

                    O SimulIDE é um ambiente de simulação
                    de circuitos eletrônicos.

                </p>

                <p>

                    Ele permite montar e testar circuitos
                    virtualmente, observando como os componentes
                    se comportam antes ou durante a montagem física.

                </p>

                <p>

                    Dessa maneira, a simulação ajuda os alunos
                    a compreender melhor os circuitos e a lógica
                    utilizada na automação.

                </p>

            </div>


        </div>

    </div>

</section>


<!-- =========================
     EXEMPLOS
========================= -->

<section class="dark-section">

    <div class="container">

        <span class="section-label">
            06 • Na prática
        </span>

        <h2 class="section-title">
            Exemplos de automação
        </h2>

        <p class="section-description">

            Veja alguns exemplos de como os componentes
            podem trabalhar juntos.

        </p>


        <div class="cards">


            <div class="card">

                <div class="card-icon">
                    🚶
                </div>

                <h3>
                    Presença
                </h3>

                <p>

                    O sensor detecta uma pessoa.
                    O Arduino recebe essa informação
                    e pode mandar acender uma iluminação.

                </p>

            </div>


            <div class="card">

                <div class="card-icon">
                    🔥
                </div>

                <h3>
                    Fumaça
                </h3>

                <p>

                    O sensor identifica fumaça.
                    O Arduino interpreta o sinal
                    e pode acionar um alerta.

                </p>

            </div>


            <div class="card">

                <div class="card-icon">
                    💧
                </div>

                <h3>
                    Nível de água
                </h3>

                <p>

                    O sensor verifica o nível da água.
                    O Arduino avalia a condição e pode
                    comandar o sistema de bombeamento.

                </p>

            </div>


        </div>

    </div>

</section>


<!-- =========================
     EQUIPE
========================= -->

<section
    class="team-section"
    id="equipe"
>

    <div class="container">

        <span class="tag">
            EET1 • CIAA
        </span>

        <h2 class="section-title">

            Projeto construído pelos alunos

        </h2>


        <div class="team-box">

            <p>

                O projeto foi construído pelos alunos:
                <strong>MN- Luciano, MN Fellipe, MN D. Raymundo,
                MN Sharon, MN Matheus, MN Gabriel, MN Macedo,
                MN Thyago, MN Maia, MN Juan Costa e o MN Junio</strong>
                como atividade prática no CIAA,
                com orientação do <strong>SO Menezes</strong>.

            </p>


            <div class="names">

                <span class="name">
                    MN- Luciano
                </span>

                <span class="name">
                    MN Fellipe
                </span>

                <span class="name">
                    MN D. Raymundo
                </span>

                <span class="name">
                    MN Sharon
                </span>

                <span class="name">
                    MN Matheus
                </span>

                <span class="name">
                    MN Gabriel
                </span>

                <span class="name">
                    MN Macedo
                </span>

                <span class="name">
                    MN Thyago
                </span>

                <span class="name">
                    MN Maia
                </span>

                <span class="name">
                    MN Juan Costa
                </span>

                <span class="name">
                    MN Junio
                </span>

            </div>


            <p>

                <strong>
                    Instrutor: SO Menezes
                </strong>

                <br>

                CIAA — Centro de Instrução Almirante Alexandrino

            </p>

        </div>

    </div>

</section>


<!-- =========================
     RODAPÉ
========================= -->

<footer>

    <strong>
        CASA INTELIGENTE • EET1
    </strong>

    <br>

    Atividade prática de Eletrônica e Automação

    <br>

    CIAA • Orientação: SO Menezes

</footer>


</body>

</html>
