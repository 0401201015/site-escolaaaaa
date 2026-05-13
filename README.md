<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jornal Estudantil | Voz da Escola</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <div class="header-top">
            <span>Brasil, 06 de Maio de 2026</span>
            <span>Edição Semanal</span>
        </div>
        <h1>O ECO ESTUDANTIL</h1>
        <p class="tagline">A voz e a inteligência da nossa comunidade escolar</p>
    </header>

    <nav>
        <ul>
            <li><a href="#">Início</a></li>
            <li><a href="#">Eventos</a></li>
            <li><a href="#">Esportes</a></li>
            <li><a href="#">Entrevistas</a></li>
            <li><a href="#">Opinião</a></li>
        </ul>
    </nav>

    <main class="container">
        <section class="main-news">
            <article>
                <img src="https://via.placeholder.com/800x400" alt="Destaque">
                <h2>Feira de Ciências 2026: Projetos Sustentáveis Surpreendem</h2>
                <p>Alunos do ensino médio apresentaram soluções inovadoras para o reaproveitamento de água da chuva no campus...</p>
                <a href="#" class="read-more">Ler mais →</a>
            </article>
        </section>

        <aside class="sidebar">
            <h3>Mais Lidas</h3>
            <div class="sidebar-item">
                <h4>Interclasse começa na próxima segunda</h4>
                <p>Prepare sua torcida! Os jogos de futsal e vôlei...</p>
            </div>
            <div class="sidebar-item">
                <h4>Cardápio do Mês</h4>
                <p>Confira as opções saudáveis do refeitório para maio.</p>
            </div>
        </aside>

        <section class="news-grid">
            <article class="grid-item">
                <h3>Clube de Xadrez</h3>
                <p>As inscrições para o torneio de inverno estão abertas até sexta.</p>
            </article>
            <article class="grid-item">
                <h3>Dicas de Estudo</h3>
                <p>Como organizar seu cronograma para as provas bimestrais.</p>
            </article>
            <article class="grid-item">
                <h3>Arte no Pátio</h3>
                <p>Exposição de grafite dos alunos do 9º ano decora os muros.</p>
            </article>
        </section>
    </main>

    <footer>
        <p>&copy; 2026 Jornal O Eco Estudantil - Produzido pela Turma de Tecnologia</p>
    </footer>

</body>
</html>

/* Configurações Gerais */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Georgia', serif; /* Fonte clássica de jornal */
}

body {
    background-color: #f4f4f4;
    color: #333;
    line-height: 1.6;
}

/* Cabeçalho */
header {
    background: #fff;
    padding: 20px 0;
    text-align: center;
    border-bottom: 4px double #000;
}

.header-top {
    display: flex;
    justify-content: space-around;
    font-size: 0.8rem;
    text-transform: uppercase;
    border-bottom: 1px solid #ddd;
    margin-bottom: 10px;
}

header h1 {
    font-size: 3.5rem;
    font-weight: 900;
    letter-spacing: -2px;
}

.tagline {
    font-style: italic;
    color: #666;
}

/* Navegação */
nav {
    background: #000;
    color: #fff;
    position: sticky;
    top: 0;
}

nav ul {
    display: flex;
    justify-content: center;
    list-style: none;
    padding: 10px 0;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
    margin: 0 15px;
    font-weight: bold;
    text-transform: uppercase;
    font-size: 0.9rem;
}

/* Layout Principal */
.container {
    max-width: 1100px;
    margin: 20px auto;
    display: grid;
    grid-template-columns: 2fr 1fr;
    gap: 20px;
    padding: 0 15px;
}

/* Notícia de Destaque */
.main-news img {
    width: 100%;
    height: auto;
    border-bottom: 5px solid #d32f2f;
}

.main-news h2 {
    font-size: 2rem;
    margin: 15px 0;
}

.read-more {
    display: inline-block;
    margin-top: 10px;
    color: #d32f2f;
    font-weight: bold;
    text-decoration: none;
}

/* Barra Lateral */
.sidebar {
    background: #fff;
    padding: 15px;
    border-left: 1px solid #ddd;
}

.sidebar h3 {
    border-bottom: 2px solid #000;
    margin-bottom: 15px;
}

.sidebar-item {
    margin-bottom: 20px;
    padding-bottom: 10px;
    border-bottom: 1px solid #eee;
}

/* Grade Inferior */
.news-grid {
    grid-column: 1 / span 2;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
    margin-top: 20px;
    border-top: 2px solid #000;
    padding-top: 20px;
}

.grid-item {
    background: #fff;
    padding: 15px;
}

/* Rodapé */
footer {
    text-align: center;
    padding: 30px;
    background: #222;
    color: #fff;
    margin-top: 40px;
}

/* Responsividade para Celular */
@media (max-width: 768px) {
    .container {
        grid-template-columns: 1fr;
    }
    .news-grid {
        grid-template-columns: 1fr;
    }
}
