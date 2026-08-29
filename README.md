# Portfólio — Kelvin Saldanha Mateus

Este é um site de portfólio pessoal multipáginas, desenvolvido com foco em performance, simplicidade e facilidade de manutenção. O projeto utiliza tecnologias web fundamentais (HTML5, CSS3 e JavaScript puro) para apresentar de forma profissional projetos, experiências, formação acadêmica e publicações.

## 🚀 Tecnologias Utilizadas

*   **HTML5:** Estrutura semântica das páginas.
*   **CSS3:** Design responsivo, animações e sistema de temas (Light/Dark Mode) via variáveis nativas.
*   **JavaScript (ES6+):** Comportamentos interativos, manipulação de DOM e lógica de configuração sem dependências externas.

## ✨ Funcionalidades Principais

*   **Modo Escuro (Dark Mode):** Suporte nativo com detecção de preferência do sistema e persistência via `localStorage`.
*   **Design Responsivo:** Otimizado para diferentes dispositivos, desde celulares pequenos até monitores desktop.
*   **Interatividade:**
    *   Menu mobile intuitivo com suporte a gestos e teclado (tecla Escape).
    *   Animações de surgimento (*fade-in*) ao rolar a página utilizando `Intersection Observer`.
    *   Sistema de "Ver Mais" para a seção de publicações.
    *   Botão "Voltar ao Topo" dinâmico.
*   **Acessibilidade e SEO:** Inclui links de salto (*skip-links*), tratamento de erros de imagem (fallback), arquivo `robots.txt` e `sitemap.xml`.
*   **Página 404 Personalizada:** Experiência de erro amigável e funcional.

## 📁 Estrutura do Projeto

A organização dos arquivos foi pensada para ser modular e fácil de navegar:

```text
/
├── index.html          # Página inicial (Home)
├── sobre.html          # Sobre o autor
├── projetos.html       # Galeria de projetos
├── experiencias.html   # Trajetória profissional
├── formacao.html       # Educação e cursos
├── conquistas.html     # Prêmios e reconhecimentos
├── publicacoes.html    # Artigos e posts
├── contato.html        # Canais de comunicação
├── 404.html            # Página de erro não encontrada
├── style.css           # Estilização global e responsividade
├── script.js           # Lógica, animações e configurações
├── sitemap.xml         # Mapa do site para SEO
├── robots.txt          # Instruções para rastreadores
└── images/             # Ativos visuais organizados por categoria
    ├── profile/        # Fotos de perfil
    ├── projects/       # Imagens dos projetos
    └── posts/          # Imagens das publicações
```


## 🛠️ Como Customizar

O projeto foi construído para que alterações de dados básicos não exijam conhecimento profundo de código.

### 1. Configurações Globais
No início do arquivo `script.js`, existe um objeto `SITE_CONFIG`. Altere-o para atualizar seu nome, links sociais e ano atual em todo o site automaticamente.

### 2. Cores e Identidade Visual
As cores do site (ambos os temas) podem ser alteradas no topo do arquivo `style.css`, dentro da seção `:root` e `[data-theme="light"]`.

### 3. Conteúdo (Textos e Imagens)
*   **Textos:** Devem ser editados diretamente nos arquivos `.html` correspondentes.
*   **Fotos:** Para trocar a foto de perfil, basta substituir o arquivo em `images/profile/` ou alterar o caminho no HTML.
*   **Novos Projetos/Publicações:** Basta copiar um bloco existente de `<article>` (ex: `projeto-card` ou `post-card`), colar abaixo e atualizar as informações de imagem e texto.

## 📦 Implantação (Deployment)

O site é estático e pode ser hospedado gratuitamente no **GitHub Pages**:
1. Crie um repositório chamado `seu-usuario.github.io`.
2. Suba todos os arquivos da pasta raiz para o repositório.
3. O site estará disponível automaticamente no endereço do repositório.

---

**Autor:** Kelvin Saldanha Mateus
**Status do Projeto:** Ativo/Atualizado
