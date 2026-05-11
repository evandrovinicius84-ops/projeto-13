# projeto-13
<!DOCTYPE html>

<html>
    <head>
        <title>Project 13</title>
        <link rel="stylesheet" href="styles.css" />
        <link rel="icon" href="favicon.ico" type="image/x-icon" />
        <script type="text/javascript" src="script.js"></script>
    </head>

    <body>
        <!-- Add HTML markup elements for your web site below -->
        <h2>bem vindo ao projeto 13!</h2>
        <div>tentando criar uma pagina simples html com ccs e banco de dados</div>
    </body>
  
</body>
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Meu Portal de Entretenimento</title>
    <!-- CSS Externo: Reset de Eric Meyer -->
    <link rel="stylesheet" href="reset.css">
    <!-- CSS Externo: Estilo Principal -->
    <link rel="stylesheet" href="style.css">
    
    <style>
        /* CSS Interno */
        body {
            background-color: #f0f2f5;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            padding: 20px;
        }
        
        /* Uso de ID para o container Flexbox */
        #main-container {
            display: flex;
            justify-content: space-between;
            gap: 20px;
            margin-top: 30px;
        }
    </style>
</head>
<body>

    <!-- CSS Inline aplicado no Header -->
    <header style="text-align: center; margin-bottom: 40px; border-bottom: 2px solid #333;">
        <h1>Meu Portal de Entretenimento Digital</h1>
    </header>

    <main id="main-container">
        <!-- Seção 1 -->
        <section class="card-entretenimento">
            <h2 class="titulo-secao">Filmes e Séries</h2>
            <p>As melhores críticas e lançamentos do cinema mundial.</p>
            <img src="https://picsum.photos" alt="Cinema" class="img-portal">
            <img src="https://picsum.photos" alt="Streaming" class="img-portal">
        </section>

        <!-- Seção 2 -->
        <section class="card-entretenimento">
            <h2 class="titulo-secao">Música e Podcasts</h2>
            <p>Sintonize nas tendências e ouça as vozes do momento.</p>
            <img src="https://picsum.photos" alt="Audio" class="img-portal">
            <img src="https://picsum.photos" alt="Headphone" class="img-portal">
        </section>

        <!-- Seção 3 -->
        <section class="card-entretenimento">
            <h2 class="titulo-secao">Games e Tecnologia</h2>
            <p>O futuro do hardware e as novidades do mundo gamer.</p>
            <img src="https://picsum.photos" alt="Controle" class="img-portal">
            <img src="https://picsum.photos" alt="Código" class="img-portal">
        </section>
    </main>
    <!-- Botão flutuante para trocar o tema -->
<button id="theme-toggle" style="position: fixed; top: 20px; right: 20px; z-index: 1000; padding: 10px; cursor: pointer;">🌓 Alternar Tema</button>

<!-- Estrutura da Modal para ampliar imagens -->
<div id="modal-imagem" class="modal">
    <span class="fechar-modal">&times;</span>
    <img id="img-ampliada" src="" alt="Imagem Ampliada">
</div>

<!-- Link para o arquivo JS -->
<script src="script.js"></script>


</body>
</html>



</html>


</html>
/* http://meyerweb.com 
   v2.0 | 20110126 | License: none (public domain) */
html, body, div, span, h1, h2, p, img, section, main {
	margin: 0;
	padding: 0;
	border: 0;
	font-size: 100%;
	font: inherit;
	vertical-align: baseline;
}
/* HTML5 display-role reset for older browsers */
main, section {
	display: block;
}
body {
	line-height: 1;
}







/* Estilização das seções (Cards) */
.card-entretenimento {
    flex: 1; /* Faz com que as colunas ocupem o mesmo espaço */
    background: #fff;
    padding: 15px;
    border-radius: 8px;
    box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    text-align: center;
}

/* Padronização dos títulos via Classe */
.titulo-secao {
    color: #2c3e50;
    font-size: 1.5rem;
    margin-bottom: 15px;
    text-transform: uppercase;
}

/* Padronização das Imagens */
.img-portal {
    width: 100%;
    height: auto;
    margin-top: 10px;
    border-radius: 5px;
    transition: transform 0.3s; /* Efeito suave ao passar o mouse */
}

.img-portal:hover {
    transform: scale(1.05);
}
/* Add CSS styles for your web site here and use them in index.html. */


<style>
    /* CSS Interno */
    body {
        /* Gradiente moderno de fundo */
        background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
        color: #fff;
        min-height: 100vh;
        padding: 40px 20px;
    }

    #main-container {
        display: flex;
        justify-content: center;
        align-items: stretch; /* Garante que todos os cards tenham a mesma altura */
        gap: 25px;
        max-width: 1200px;
        margin: 0 auto;
        /* Permite que os cards quebrem de linha em telas pequenas */
        flex-wrap: wrap; 
    }
</style>



/* --- Estilização dos Cards com Efeito Glassmorphism --- */
.card-entretenimento {
    flex: 1;
    min-width: 300px; /* Impede que o card fique muito estreito */
    background: rgba(255, 255, 255, 0.05); /* Fundo semi-transparente */
    backdrop-filter: blur(10px); /* Efeito de vidro embaçado */
    padding: 25px;
    border-radius: 15px;
    border: 1px dotted rgba(255, 255, 255, 0.1);
    box-shadow: 0 8px 32px rgba(0, 0, 0, 0.3);
    text-align: center;
    transition: all 0.4s ease;
}

/* Efeito de destaque ao passar o mouse no Card */
.card-entretenimento:hover {
    background: rgba(255, 255, 255, 0.1);
    transform: translateY(-10px); /* Move o card levemente para cima */
    border-color: #4ecca3;
}

/* --- Títulos das Seções --- */
.titulo-secao {
    color: #4ecca3; /* Verde neon tecnológico */
    font-size: 1.6rem;
    font-weight: bold;
    margin-bottom: 20px;
    letter-spacing: 1px;
    border-bottom: 2px solid rgba(78, 204, 163, 0.3);
    padding-bottom: 10px;
}

/* --- Estilização das Imagens --- */
.img-portal {
    width: 100%;
    height: 160px;
    object-fit: cover; /* Mantém a proporção sem distorcer */
    margin-top: 15px;
    border-radius: 10px;
    filter: grayscale(30%); /* Efeito leve de cor */
    transition: filter 0.3s ease;
}

.img-portal:hover {
    filter: grayscale(0%); /* Volta a cor total no hover */
}

/* --- Texto Explicativo --- */
p {
    font-size: 0.95rem;
    color: #567488;
    line-height: 1.5;
    margin-bottom: 20px;
}
/* Estilo para a Modal (Janela de Zoom) */
.modal {
    display: none; /* Escondida por padrão */
    position: fixed;
    z-index: 2000;
    left: 0; top: 0; width: 100%; height: 100%;
    background-color: rgba(0,0,0,0.9);
    justify-content: center;
    align-items: center;
}

.modal img {
    max-width: 80%;
    max-height: 80%;
    border: 3px solid #4ecca3;
    border-radius: 10px;
}

.fechar-modal {
    position: absolute;
    top: 30px; right: 50px;
    color: white; font-size: 40px; cursor: pointer;
}

/* Classe para o Modo Claro (ativada via JS) */
body.light-mode {
    background: #f4f4f4;
    color: #333;
}
body.light-mode .card-entretenimento {
    background: white;
    color: #333;
    border-color: #ddd;
}

<?php
// Configurações do banco de dados
$host = 'localhost';
$db   = 'portal_entretenimento';
$user = 'root'; // ajuste conforme seu ambiente
$pass = '';     // ajuste conforme seu ambiente

try {
    $pdo = new PDO("mysql:host=$host;dbname=$db;charset=utf8", $user, $pass);
    
    // Consulta para buscar os conteúdos e suas respectivas imagens
    // Usamos um JOIN para trazer tudo de uma vez
    $sql = "SELECT c.id, c.titulo_card, c.texto_explicativo 
            FROM conteudos c";
    $query = $pdo->query($sql);
    $secoes = $query->fetchAll(PDO::FETCH_ASSOC);

} catch (PDOException $e) {
    die("Erro ao conectar: " . $e->getMessage());
}
?>

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Meu Portal Dinâmico</title>
    <link rel="stylesheet" href="reset.css">
    <link rel="stylesheet" href="style.css">
    <!-- O CSS Interno que criamos anteriormente vai aqui -->
    <style>
        body {
            background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
            color: #fff;
            min-height: 100vh;
            padding: 40px 20px;
            font-family: sans-serif;
        }
        #main-container {
            display: flex;
            justify-content: center;
            gap: 25px;
            max-width: 1200px;
            margin: 0 auto;
            flex-wrap: wrap;
        }
    </style>
</head>
<body>

    <header style="text-align: center; margin-bottom: 40px; border-bottom: 2px solid #4ecca3;">
        <h1>Meu Portal de Entretenimento Digital</h1>
    </header>

    <main id="main-container">
        <?php foreach ($secoes as $secao): ?>
            <section class="card-entretenimento">
                <h2 class="titulo-secao"><?php echo htmlspecialchars($secao['titulo_card']); ?></h2>
                <p><?php echo htmlspecialchars($secao['texto_explicativo']); ?></p>
                
                <div class="galeria-fotos">
                    <?php
                    // Busca as imagens específicas desta seção
                    $stmtImg = $pdo->prepare("SELECT url_imagem, legenda FROM imagens WHERE conteudo_id = ?");
                    $stmtImg->execute([$secao['id']]);
                    $imagens = $stmtImg->fetchAll(PDO::FETCH_ASSOC);

                    foreach ($imagens as $img): ?>
                        <img src="<?php echo $img['url_imagem']; ?>" 
                             alt="<?php echo $img['legenda']; ?>" 
                             class="img-portal">
                    <?php endforeach; ?>
                </div>
            </section>
        <?php endforeach; ?>
    </main>

</body>
</html>
// 1. Efeito de Revelação (Scroll Reveal)
// Faz as seções aparecerem suavemente ao carregar a página
document.addEventListener("DOMContentLoaded", () => {
    const cards = document.querySelectorAll('.card-entretenimento');
    cards.forEach((card, index) => {
        setTimeout(() => {
            card.style.opacity = "1";
            card.style.transform = "translateY(0)";
        }, 200 * index); // Delay cascata para cada card
    });
});

// 2. Alternador de Tema (Dark/Light Mode)
const themeBtn = document.getElementById('theme-toggle');
themeBtn.addEventListener('click', () => {
    document.body.classList.toggle('light-mode');
    // Salva a preferência do usuário no navegador
    const isLight = document.body.classList.contains('light-mode');
    localStorage.setItem('theme', isLight ? 'light' : 'dark');
});

// 3. Sistema de Modal (Zoom na Imagem)
const modal = document.getElementById('modal-imagem');
const modalImg = document.getElementById('img-ampliada');
const imagens = document.querySelectorAll('.img-portal');
const btnFechar = document.querySelector('.fechar-modal');

// Abre a modal ao clicar em qualquer imagem do portal
imagens.forEach(img => {
    img.addEventListener('click', () => {
        modal.style.display = "flex";
        modalImg.src = img.src;
    });
});

// Fecha a modal ao clicar no 'X' ou fora da imagem
btnFechar.onclick = () => modal.style.display = "none";
window.onclick = (event) => {
    if (event.target == modal) modal.style.display = "none";
};
