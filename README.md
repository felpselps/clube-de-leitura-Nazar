<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
    <title>Clube de Leitura Nazar</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            background-color: #FFFFFF;
            color: #333333;
            line-height: 1.6;
        }

        header {
            background: linear-gradient(to right, #6A1B9A, #8E24AA);
            color: white;
            padding: 50px 20px;
            text-align: center;
        }

        nav {
            background-color: #E1BEE7;
            padding: 12px 0;
            text-align: center;
            position: sticky;
            top: 0;
            z-index: 999;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }

        nav a {
            color: #4A0072;
            font-weight: 600;
            text-decoration: none;
            margin: 0 20px;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #6A1B9A;
        }

        section {
            padding: 60px 20px;
            max-width: 1000px;
            margin: auto;
        }

        section:nth-child(even) {
            background-color: #F3E5F5;
        }

        h2 {
            margin-bottom: 20px;
            color: #6A1B9A;
        }

        .livro {
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 12px rgba(106, 27, 154, 0.1);
            margin-bottom: 25px;
        }

        .livro h3 {
            color: #4A0072;
            margin-bottom: 10px;
        }

        .btn {
            display: inline-block;
            background-color: #8E24AA;
            color: white;
            padding: 12px 24px;
            border-radius: 6px;
            text-decoration: none;
            margin-top: 15px;
            font-weight: 600;
            transition: background-color 0.3s;
        }

        .btn:hover {
            background-color: #6A1B9A;
        }

        a {
            color: #6A1B9A;
        }

        a:hover {
            text-decoration: underline;
        }

        footer {
            background-color: #6A1B9A;
            color: white;
            text-align: center;
            padding: 20px;
        }

        /* Estilo específico para o cronograma */
        .cronograma {
            background-color: white;
            padding: 25px 30px;
            border-radius: 10px;
            box-shadow: 0 4px 12px rgba(106, 27, 154, 0.1);
            max-width: 500px;
            margin: auto;
            font-size: 1.1rem;
            color: #4A0072;
        }

        .cronograma p {
            margin-bottom: 10px;
        }

        .data {
            font-weight: 700;
            color: #6A1B9A;
        }

        /* Barra de progresso */
        .progress-container {
            background-color: #E1BEE7;
            border-radius: 12px;
            overflow: hidden;
            margin-top: 20px;
            height: 25px;
            width: 100%;
            max-width: 500px;
            margin-left: auto;
            margin-right: auto;
            box-shadow: inset 0 1px 3px rgba(0,0,0,0.2);
        }

        .progress-bar {
            background: linear-gradient(90deg, #8E24AA, #6A1B9A);
            height: 100%;
            width: 0%;
            transition: width 1s ease-in-out;
        }

        .progress-text {
            text-align: center;
            margin-top: 8px;
            font-weight: 600;
            color: #6A1B9A;
        }
    </style>
</head>
<body>

    <header>
        <h1>Clube de Leitura Nazar</h1>
        <p>Descubra, leia e compartilhe suas histórias favoritas!</p>
    </header>

    <nav>
        <a href="#sobre">Sobre</a>
        <a href="#livros">Livro do Mês</a>
        <a href="#cronograma">Cronograma</a>
        <a href="#contato">Contato</a>
    </nav>

    <section id="sobre">
        <h2>Sobre o Clube</h2>
        <p>O Clube do Livro Escolar é um espaço para alunos que amam leitura! Compartilhamos obras incríveis, debatemos temas atuais e incentivamos a criatividade através dos livros.</p>
    </section>

    <section id="livros">
        <h2>Livro do Mês</h2>

        <div class="livro">
            <h3>Ainda Estou Aqui – Marcelo Rubens Paiva</h3>
            <p>Uma emocionante autobiografia que mistura história, política e memória familiar, escrita por um dos autores mais importantes da literatura brasileira contemporânea.</p>
            <a href="https://drive.google.com/file/d/1hcfzjcfRkfNpQKf7hquKoApo439BkaUJ/view?usp=drive_link" target="_blank" class="btn">Ler PDF</a>
        </div>
    </section>

    <section id="cronograma">
        <h2>Cronograma de Leitura</h2>
        <div class="cronograma">
            <p>📅 <strong>Início da leitura:</strong> <span class="data">13/05</span></p>
            <p>⏰ <strong>Prazo para finalização:</strong> <span class="data">13/06</span></p>
            <p>🎉 <strong>Revelação do próximo livro:</strong> <span class="data">16/06</span></p>

            <div class="progress-container" aria-label="Progresso da leitura">
                <div class="progress-bar" id="progress-bar"></div>
            </div>
            <div class="progress-text" id="progress-text">Calculando progresso...</div>
        </div>
    </section>

    <section id="contato">
        <h2>Entre em Contato</h2>
        <p>Email: <a href="mailto:brunopreda@professor.educacão.sp.gov.br">brunopreda@professor.educacão.sp.gov.br</a></p>
        <p>Instagram: <a href="https://www.instagram.com/saladeleituranazar?igsh=MW03cThmYWpqZm1leA==" target="_blank">@saladeleituranazar</a></p>
    </section>

    <footer>
        <p>&copy; 2025 Clube de Leitura Nazar. Todos os direitos reservados.</p>
    </footer>

    <script>
        // Datas importantes
        const inicioLeitura = new Date('2025-05-13T00:00:00');
        const fimLeitura = new Date('2025-06-13T23:59:59');

        // Elementos da barra e texto
        const progressBar = document.getElementById('progress-bar');
        const progressText = document.getElementById('progress-text');

        function atualizarProgresso() {
            const hoje = new Date();

            if (hoje < inicioLeitura) {
                // Antes do início
                progressBar.style.width = '0%';
                progressText.textContent = 'A leitura ainda não começou.';
            } else if (hoje > fimLeitura) {
                // Depois do fim
                progressBar.style.width = '100%';
                progressText.textContent = 'Prazo de leitura finalizado!';
            } else {
                // Durante o período de leitura
                const duracaoTotal = fimLeitura - inicioLeitura;
                const duracaoPassada = hoje - inicioLeitura;
                const progresso = (duracaoPassada / duracaoTotal) * 100;

                progressBar.style.width = progresso.toFixed(2) + '%';
                progressText.textContent = `Progresso da leitura: ${progresso.toFixed(1)}%`;
            }
        }

        atualizarProgresso();

        // Atualiza a cada minuto para manter sincronizado
        setInterval(atualizarProgresso, 60000);
    </script>

</body>
</html>
