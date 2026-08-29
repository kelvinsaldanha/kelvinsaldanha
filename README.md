# Portfólio — Kelvin Saldanha Mateus

[![Status](https://img.shields.io/badge/status-ativo-brightgreen)](https://github.com/Kelvinsaldanha/portfolio)
[![Tecnologias](https://img.shields.io/badge/HTML5-CSS3-blue)](https://github.com/Kelvinsaldanha/portfolio)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6%2B-yellow)](https://github.com/Kelvinsaldanha/portfolio)

---

## 📋 Visão Geral

Este é um site de portfólio pessoal multipáginas, desenvolvido para apresentar de forma profissional a trajetória, projetos, experiências, formação acadêmica e publicações de **Kelvin Saldanha Mateus** — estudante de Equipamentos Biomédicos no CEFET-MG.

O projeto utiliza **tecnologias web fundamentais** (HTML5, CSS3 e JavaScript puro), sem dependências externas, garantindo:

- ✅ **Performance** — Código leve e otimizado para carregamento rápido.
- ✅ **Simplicidade** — Estrutura clara e bem organizada para fácil manutenção.
- ✅ **Acessibilidade** — Links de salto (`skip-links`), atributos ARIA e navegação por teclado.
- ✅ **SEO** — Dados estruturados (JSON-LD), `sitemap.xml` e `robots.txt` configurados.
- ✅ **Design responsivo** — Experiência consistente em todos os dispositivos, de smartphones a monitores desktop.

---

## 🚀 Tecnologias Utilizadas

| Tecnologia | Descrição |
|------------|-----------|
| **HTML5** | Estrutura semântica das páginas, garantindo acessibilidade e SEO. |
| **CSS3** | Design responsivo, animações suaves e sistema de temas (Light/Dark Mode) via variáveis nativas CSS. |
| **JavaScript (ES6+)** | Comportamentos interativos, manipulação de DOM, lógica de configuração e animações com `Intersection Observer`. |

### Bibliotecas Externas (Leves e CDN)

| Recurso | Finalidade |
|---------|------------|
| **[Google Fonts (Inter)](https://fonts.google.com/specimen/Inter)** | Tipografia moderna e legível para todo o site. |
| **[Devicon](https://devicon.dev/)** | Ícones de tecnologias utilizados na página de habilidades técnicas. |

---

## ✨ Funcionalidades Principais

### 🌓 Modo Escuro (Dark Mode)

- Suporte nativo com detecção da preferência do sistema (`prefers-color-scheme`).
- Persistência da escolha do usuário via `localStorage`.
- Alternância suave com ícone dinâmico (🌙/☀️) no menu de navegação.

### 📱 Design Responsivo

- Otimizado para diferentes dispositivos — desde celulares pequenos (320px) até monitores desktop (1440px+).
- Menu mobile intuitivo com suporte a gestos de toque e teclado (tecla **Escape** para fechar).
- Grids flexíveis que se adaptam automaticamente ao tamanho da tela.

### 🎯 Interatividade e Animações

- **Animações de surgimento (`fade-in`)** — Utiliza `Intersection Observer` para animar elementos conforme o usuário rola a página.
- **Sistema "Ver Mais"** — Na seção de publicações, exibe inicialmente 6 posts e permite carregar o restante com um clique.
- **Botão "Voltar ao Topo"** — Aparece dinamicamente após rolar a página e rola suavemente até o topo.
- **Lightbox (Galeria de Imagens)** — Modal para ampliar imagens com navegação por teclado (setas) e contador de imagens.

### ♿ Acessibilidade e SEO

- **Links de salto (`skip-links`)** — Permite que usuários de leitores de tela pulem diretamente para o conteúdo principal.
- **Atributos ARIA** — Navegação com `aria-expanded`, `aria-controls`, `aria-label` e `role="dialog"` para o lightbox.
- **Tratamento de erros de imagem (fallback)** — Exibe "Imagem indisponível" para imagens quebradas.
- **Arquivos de SEO** — `robots.txt` e `sitemap.xml` para otimização em mecanismos de busca.
- **Dados Estruturados (JSON-LD)** — Schema.org para Person, ProfilePage, Article e Achievement.
- **Página 404 Personalizada** — Experiência de erro amigável com links úteis para navegação.

### 📸 Galeria Lightbox

- Clique em qualquer imagem da galeria de figuras para ampliá-la.
- Navegação com setas (← →) ou teclado.
- Contador de imagens e legenda exibida abaixo da imagem ampliada.
- Fechar com clique fora da imagem, botão ✕ ou tecla **Escape**.

---

## 📁 Estrutura do Projeto

A organização dos arquivos foi pensada para ser **modular e fácil de navegar**:

```text
/
├── README.md                           # Documentação do projeto
│
├── Páginas principais
│   ├── index.html                      # Página inicial (Home)
│   ├── sobre.html                      # Sobre o autor
│   ├── habilidades.html                # Habilidades técnicas
│   ├── projetos.html                   # Galeria de projetos
│   ├── experiencias.html               # Trajetória profissional
│   ├── formacao.html                   # Educação e cursos
│   ├── publicacoes.html                # Artigos e posts
│   ├── conquistas.html                 # Prêmios e reconhecimentos
│   ├── contato.html                    # Canais de comunicação
│   └── 404.html                        # Página de erro não encontrada
│
├── Páginas detalhadas de projetos
│   └── guia-respiracao.html            # Página detalhada do projeto Guia de Respiração
│
├── Arquivos de configuração e SEO
│   ├── style.css                       # Estilização global e responsividade
│   ├── script.js                       # Lógica, animações e configurações
│   ├── sitemap.xml                     # Mapa do site para SEO
│   ├── robots.txt                      # Instruções para rastreadores
│   └── google784ac2a023e58c0a.html     # Verificação de propriedade Google Search Console
│
└── images/                             # Ativos visuais organizados por categoria
    ├── profile/                        # Fotos de perfil
    ├── projects/                       # Imagens dos projetos
    │   └── guia-respiracao/            # Imagens específicas do projeto Guia de Respiração
    └── posts/                          # Imagens das publicações
🛠️ Como Customizar
O projeto foi construído para que alterações de dados básicos não exijam conhecimento profundo de código. Abaixo estão as principais áreas de personalização:

1. Configurações Globais
No início do arquivo script.js, existe um objeto SITE_CONFIG. Altere-o para atualizar nome, links sociais e ano atual em todo o site automaticamente:

javascript
const SITE_CONFIG = {
    name: "Kelvin Saldanha Mateus",
    github: "https://github.com/Kelvinsaldanha",
    linkedin: "https://www.linkedin.com/in/kelvin-saldanha-mateus/",
    email: "kelvinsaldanhaa@gmail.com",
    currentYear: 2026
};
2. Cores e Identidade Visual
As cores do site (ambos os temas) podem ser alteradas no topo do arquivo style.css:

Modo Escuro: dentro da seção :root

Modo Claro: dentro da seção [data-theme="light"]

css
:root {
    --color-background: #0a0e1a;
    --color-primary: #3b82f6;
    /* ... */
}

[data-theme="light"] {
    --color-background: #ffffff;
    --color-primary: #2563eb;
    /* ... */
}
3. Conteúdo (Textos e Imagens)
Tipo	Como alterar
Textos	Editar diretamente nos arquivos .html correspondentes.
Foto de perfil	Substituir o arquivo em images/profile/ ou alterar o caminho no HTML.
Novos Projetos	Copiar um bloco <article class="projeto-card"> em projetos.html, colar abaixo e atualizar imagem, título, descrição, tecnologias e status.
Novas Publicações	Copiar um bloco <article class="post-card"> em publicacoes.html e atualizar imagem, categoria, data, título, resumo e link.
Novas Habilidades	Copiar um bloco <div class="habilidade-card"> em habilidades.html e atualizar ícone (classe Devicon), título e descrição.
Certificados	Copiar um bloco <article class="certificado-card"> em conquistas.html e atualizar imagem, título, instituição e ano.
4. Adicionar uma Nova Página
Crie um novo arquivo .html na raiz.

Copie a estrutura do cabeçalho (header) e rodapé (footer) de uma página existente.

Adicione um link para a nova página no menu de navegação (<ul class="nav__menu">).

Atualize o sitemap.xml com a nova URL.

📦 Implantação (Deployment)
O site é estático e pode ser hospedado gratuitamente em diversas plataformas:

GitHub Pages
Crie um repositório chamado seu-usuario.github.io.

Suba todos os arquivos da pasta raiz para o repositório.

O site estará disponível automaticamente em https://seu-usuario.github.io/.

Vercel / Netlify
Conecte seu repositório GitHub à plataforma escolhida.

A implantação será automática a cada push na branch principal.

Configuração recomendada: pasta raiz como diretório de publicação.

Hospedagem Tradicional
Faça upload de todos os arquivos para o diretório público do seu servidor via FTP.

Certifique-se de que o servidor sirva index.html como página inicial.

📄 Licença
Este projeto é de uso pessoal e educacional. Fique à vontade para usá-lo como referência para seu próprio portfólio.

👤 Autor
Kelvin Saldanha Mateus

E-mail: kelvinsaldanhaa@gmail.com

GitHub: github.com/Kelvinsaldanha

LinkedIn: linkedin.com/in/kelvin-saldanha-mateus

📊 Status do Projeto
Versão: 2.0

Status: ✅ Ativo / Atualizado

Última atualização: Agosto 2026

📚 Referências e Agradecimentos
Google Fonts — Fontes utilizadas no projeto.

Devicon — Ícones de tecnologias.

MDN Web Docs — Documentação de referência para HTML, CSS e JavaScript.

Feito com 💙 por Kelvin Saldanha Mateus.
