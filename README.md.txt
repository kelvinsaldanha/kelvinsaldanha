# Portfólio — Kelvin Saldanha Mateus

Site portfólio pessoal desenvolvido com HTML5, CSS3 e JavaScript puro.  
O objetivo é apresentar projetos, experiências, formação e publicações de forma profissional e fácil de manter.

## 1. Sobre o projeto

Este portfólio foi criado para ser simples, rápido e fácil de editar, mesmo para quem não tem conhecimento avançado em programação.  
Ele é totalmente estático e pode ser hospedado gratuitamente no GitHub Pages.

## 2. Estrutura de arquivos

```
/
├── index.html
├── style.css
├── script.js
├── README.md
├── .gitignore
└── images/
    ├── profile/
    ├── projects/
    └── posts/
```

- **index.html** — contém todo o conteúdo e estrutura do site.
- **style.css** — toda a aparência (cores, tipografia, layout, responsividade).
- **script.js** — comportamentos interativos (menu, dark mode, ver mais, animações).
- **images/** — pasta para guardar todas as imagens organizadas por tipo.

## 3. Como abrir

Basta abrir o arquivo `index.html` diretamente no navegador (duplo clique).  
Opcionalmente, você pode usar a extensão **Live Server** no VS Code para visualizar com atualização automática.

## 4. Como adicionar sua foto

1. Coloque sua foto no formato JPG ou PNG dentro da pasta `images/profile/`.
2. Renomeie o arquivo para `kelvin.jpg` (ou mantenha o nome e altere no HTML).
3. A foto será exibida automaticamente no topo do site.

Se a foto não for encontrada, o site mostrará um espaço elegante com a palavra "Foto de perfil" (sem quebrar o layout).

## 5. Como adicionar um projeto

1. Abra o arquivo `index.html` em um editor de texto.
2. Procure pela seção **Projetos** (comentário `<!-- PROJETO 01 ... -->`).
3. Copie um bloco completo de `<article class="projeto-card">...</article>`.
4. Cole logo abaixo do último projeto, antes do comentário de instruções.
5. Altere:
   - `src="images/projects/nome-da-imagem.jpg"` para o caminho da nova imagem.
   - `alt` para uma descrição da imagem.
   - Título, descrição, tecnologias (`<li>`), status e link, se houver.
6. Salve o arquivo.

Não é necessário alterar o CSS ou JavaScript. O layout se ajusta automaticamente.

## 6. Como adicionar uma publicação

1. Coloque a imagem da publicação na pasta `images/posts/` (ex: `minha-publicacao.jpg`).
2. No `index.html`, localize a seção **Publicações**.
3. Copie um bloco `<article class="post-card">...</article>`.
4. Cole logo abaixo do último card, antes do comentário de instruções.
5. Altere:
   - `src="images/posts/minha-publicacao.jpg"` para o caminho da imagem.
   - `alt`, categoria, data, título, resumo e link.
6. Salve.

O botão "Ver mais" funciona automaticamente: se houver mais de 6 publicações, as extras ficarão ocultas até o clique.

## 7. Como adicionar qualquer imagem

- Fotos de perfil: coloque em `images/profile/`.
- Imagens de projetos: coloque em `images/projects/`.
- Imagens de publicações: coloque em `images/posts/`.

Use nomes simples e sem espaços (ex: `eye-tracker.jpg`, `expo-hospital-2026.jpg`).  
Evite nomes como `IMG_20260817_183928_FINAL_FINAL2.jpg` — prefira algo curto e descritivo.

Formatos recomendados:
- **JPG** para fotos;
- **PNG** para imagens com transparência;
- **WebP** quando possível (mais leve).

## 8. Como publicar no GitHub Pages

1. Crie um repositório no GitHub com o nome `seu-usuario.github.io` (substitua `seu-usuario` pelo seu nome de usuário).
2. Faça o upload de todos os arquivos (incluindo a pasta `images/`) para o repositório.
3. No GitHub, vá em **Settings** → **Pages**.
4. Em **Branch**, selecione `main` (ou `master`) e pasta `/ (root)`.
5. Clique em **Save**.
6. Aguarde alguns minutos. O site estará disponível em `https://seu-usuario.github.io`.

## 9. Como atualizar o site

Após editar os arquivos localmente:

1. Salve as alterações.
2. No repositório GitHub, clique em **Add file** → **Upload files** (ou use Git).
3. Envie os arquivos modificados.
4. O GitHub Pages atualiza automaticamente em poucos minutos.

Fluxo resumido:

```
editar → salvar → GitHub → Commit → GitHub Pages atualiza
```

## 10. Personalização rápida

- **Cores**: edite as variáveis CSS no topo do `style.css` (seção `:root`).
- **Nome e links**: altere o objeto `SITE_CONFIG` no início do `script.js`.
- **Textos**: edite diretamente no `index.html`.

Qualquer dúvida, consulte os comentários nos próprios arquivos.