/* ====== Reset básico para remover margens e definir fonte ====== */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box; /* Inclui bordas no cálculo total de largura/altura */
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

/* ====== Estilos gerais do corpo ====== */
body {
  background-color: #0D1B2A; /* Azul escuro de fundo */
  color: #E0E0E0;           /* Texto em cinza claro */
  line-height: 2.0;         /* Altura da linha para melhor leitura */
}

/* ====== Cabeçalho ====== */
header {
  background-color: #1A3C40; /* Fundo verde-azulado escuro */
  padding: 20px;
  text-align: center;
}

header h1 {
  font-size: 2.5rem;  /* Título grande */
  color: #F5F5F5;     /* Cor clara no título */
}

/* ====== Navegação ====== */
nav {
  background-color: #162938; /* Cor de fundo do menu */
  display: flex;            /* Flexbox para alinhar links na horizontal */
  justify-content: center;  /* Centraliza os links */
  padding: 10px 0;
}

nav a {
  color: #E0E0E0;           /* Cor dos links */
  text-decoration: none;    /* Remove o sublinhado */
  margin: 0 20px;           /* Espaço entre links */
  font-weight: bold;
  transition: color 0.3s;   /* Efeito suave ao passar o mouse */
}

nav a:hover {
  color: #FFD700;           /* Muda para dourado ao passar o mouse */
}

/* ====== Seções ====== */
section {
  padding: 40px 20px;       /* Espaço interno da seção */
  max-width: 1200px;        /* Limita a largura máxima */
  margin: auto;             /* Centraliza o conteúdo */
}

section h2 {
  color: #FFD700;           /* Títulos em dourado */
  margin-bottom: 20px;
  font-size: 2rem;
  border-bottom: 2px solid #FFD700; /* Linha dourada abaixo do título */
  display: inline-block;    /* A linha ocupa apenas a largura do texto */
  padding-bottom: 5px;
}

/* ====== Grades (grid) de cards ====== */
.news, .highlights, .calendar {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); /* Ajusta as colunas automaticamente */
  gap: 20px; /* Espaçamento entre cards */
}

/* ====== Estilo de cada card ====== */
.card {
  background-color: #1C2A3A; /* Fundo do card */
  padding: 15px;
  border-radius: 10px;       /* Bordas arredondadas */
  transition: transform 0.3s; /* Efeito suave ao passar o mouse */
}

.card:hover {
  transform: scale(1.05);   /* Leve zoom ao passar o mouse */
}

.card h3 {
  color: #FFD700;           /* Título do card em dourado */
  margin-bottom: 10px;
}

.card p {
  font-size: 0.9rem;        /* Texto um pouco menor */
  color: #F0F0F0;
}

/* ====== Rodapé ====== */
footer {
  background-color: #1A3C40; /* Mesma cor do cabeçalho para consistência */
  text-align: center;
  padding: 20px;
  margin-top: 40px;
}

footer p {
  color: #E0E0E0;
}

/* ====== Botão de Ação (Call To Action) ====== */
.btn {
  display: inline-block;
  padding: 10px 20px;
  background-color: #FFD700; /* Fundo dourado */
  color: #0D1B2A;           /* Texto em azul escuro */
  font-weight: bold;
  text-decoration: none;    /* Remove sublinhado */
  border-radius: 5px;
  transition: background 0.3s;
  margin-top: 10px;
}

.btn:hover {
  background-color: #e6c200; /* Dourado mais escuro no hover */
}

/* ====== Formulário de Contato ====== */
form input, form textarea {
  width: 100%;        /* Largura total */
  padding: 10px;
  margin-bottom: 15px;
  border-radius: 5px;
  border: none;
  font-size: 1rem;
}

form button {
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  background-color: #FFD700; /* Botão dourado */
  color: #0D1B2A;           /* Texto azul escuro */
  font-weight: bold;
  cursor: pointer;
  transition: background 0.3s;
}

form button:hover {
  background-color: #e6c200; /* Dourado mais escuro no hover */
}

/* ====== Melhores Momentos ====== */

#highlights {
  padding: 35px;
  background-color: #0d1b2a; /* fundo escuro */
  color: #fff;
}

#highlights h2 {
  font-size: 20px;
  margin-bottom: 20px;
  border-bottom: 3px solid #facc15; /* amarelo destaque */
  display: inline-block;
  padding-bottom: 5px;
}

/* Layout em grid para os cards */
.highlights {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
  gap: 20px;
}

/* Card de cada vídeo */
.card {
  background-color: #1e293b; /* cinza-azulado */
  border-radius: 10px;
  padding: 15px;
  box-shadow: 0px 4px 12px rgba(0,0,0,0.3);
}

/* Título dentro do card */
.card h3 {
  margin-bottom: 10px;
  font-size: 15px;
}

/* Container do vídeo responsivo */
.video-container {
  position: relative;
  padding-bottom: 56.25%; /* proporção 16:9 */
  height: 0;
  overflow: hidden;
  border-radius: 10px;
}

.video-container iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border: none;
}
