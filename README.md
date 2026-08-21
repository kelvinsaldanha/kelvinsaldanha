# Portfólio — Kelvin Saldanha Mateus

Site portfólio pessoal multipáginas desenvolvido com HTML5, CSS3 e JavaScript puro.  
O objetivo é apresentar projetos, experiências, formação e publicações de forma profissional e fácil de manter.

## Sobre

Este portfólio foi criado para ser simples, rápido e fácil de editar, mesmo para quem não tem conhecimento avançado em programação.  
Ele é totalmente estático e pode ser hospedado gratuitamente no GitHub Pages.

## Estrutura

```
/
├── index.html
├── sobre.html
├── projetos.html
├── experiencias.html
├── formacao.html
├── publicacoes.html
├── contato.html
├── style.css
├── script.js
├── README.md
├── .gitignore
└── images/
    ├── profile/
    ├── projects/
    └── posts/
```

- **index.html** — Página inicial (home).
- **sobre.html** — Página sobre Kelvin.
- **projetos.html** — Página de projetos.
- **experiencias.html** — Página de experiências.
- **formacao.html** — Página de formação.
- **publicacoes.html** — Página de publicações.
- **contato.html** — Página de contato.
- **style.css** — Toda a aparência (cores, tipografia, layout, responsividade).
- **script.js** — Comportamentos interativos (menu, dark mode, ver mais, animações).
- **images/** — Pasta para guardar todas as imagens organizadas por tipo.

## Como executar

1. Baixe ou clone este repositório.
2. Abra o arquivo `index.html` diretamente no navegador (duplo clique).
3. Opcionalmente, use a extensão **Live Server** no VS Code para visualizar com atualização automática.

## Como editar textos

Todos os textos estão nos arquivos `.html`.  
Procure pelo conteúdo que deseja alterar e edite diretamente no editor de texto.

## Como trocar a foto

1. Coloque sua foto no formato JPG ou PNG dentro da pasta `images/profile/`.
2. Renomeie o arquivo para `kelvin.jpg` (ou mantenha o nome e altere no HTML).
3. A foto será exibida automaticamente no topo do site.

Se a foto não for encontrada, o site mostrará um espaço elegante com a palavra "Foto de perfil" (sem quebrar o layout).

## Como adicionar imagem de projeto

1. Coloque a imagem na pasta `images/projects/`.
2. No arquivo `projetos.html`, copie um bloco `<article class="projeto-card">...</article>`.
3. Cole logo abaixo do último projeto, antes do comentário de instruções.
4. Altere:
   - `src="images/projects/nome-da-imagem.jpg"` para o caminho da nova imagem.
   - `alt` para uma descrição da imagem.
   - Título, descrição, tecnologias (`<li>`), status e link, se houver.
5. Salve o arquivo.

## Como adicionar publicação

1. Coloque a imagem da publicação na pasta `images/posts/` (ex: `minha-publicacao.jpg`).
2. No arquivo `publicacoes.html`, copie um bloco `<article class="post-card">...</article>`.
3. Cole logo abaixo do último card, antes do comentário de instruções.
4. Altere:
   - `src="images/posts/minha-publicacao.jpg"` para o caminho da imagem.
   - `alt`, categoria, data, título, resumo e link.
5. Salve.

O botão "Ver mais" funciona automaticamente: se houver mais de 6 publicações, as extras ficarão ocultas até o clique.

## Como adicionar uma nova página

1. Copie um arquivo HTML existente (ex: `sobre.html`).
2. Renomeie para o nome desejado (ex: `nova-pagina.html`).
3. Altere o conteúdo dentro da tag `<main>`.
4. Atualize os links da navbar e do footer em todas as páginas (ou apenas na nova página).
5. Salve.

## Como publicar no GitHub Pages

1. Crie um repositório no GitHub com o nome `seu-usuario.github.io` (substitua `seu-usuario` pelo seu nome de usuário).
2. Faça o upload de todos os arquivos (incluindo a pasta `images/`) para o repositório.
3. No GitHub, vá em **Settings** → **Pages**.
4. Em **Branch**, selecione `main` (ou `master`) e pasta `/ (root)`.
5. Clique em **Save**.
6. Aguarde alguns minutos. O site estará disponível em `https://seu-usuario.github.io`.

## Como atualizar o site

Após editar os arquivos localmente:

1. Salve as alterações.
2. No repositório GitHub, clique em **Add file** → **Upload files** (ou use Git).
3. Envie os arquivos modificados.
4. O GitHub Pages atualiza automaticamente em poucos minutos.

Fluxo resumido:

```
editar → salvar → GitHub → Commit → GitHub Pages atualiza
```

## Personalização rápida

- **Cores**: edite as variáveis CSS no topo do `style.css` (seção `:root`).
- **Nome e links**: altere o objeto `SITE_CONFIG` no início do `script.js`.
- **Textos**: edite diretamente nos arquivos `.html`.

Qualquer dúvida, consulte os comentários nos próprios arquivos.
