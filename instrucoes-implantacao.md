# Instruções de Implantação - FonoTech Landing Page

Este documento contém instruções detalhadas para implantar o site estático da FonoTech em diferentes plataformas de hospedagem gratuita.

## Estrutura do Projeto

O projeto consiste nos seguintes arquivos e diretórios:

```
fonoaudio-site/
├── index.html          # Página principal do site
├── css/
│   └── styles.css      # Estilos do site
├── js/
│   └── main.js         # JavaScript para interatividade
└── images/             # Diretório de imagens
    ├── hero-placeholder.svg
    ├── problema-placeholder.svg
    ├── solucao-placeholder.svg
    ├── beneficios-placeholder.svg
    ├── diferenciais-placeholder.svg
    ├── icon-gestao.svg
    ├── icon-financeiro.svg
    ├── icon-nfse.svg
    └── icon-lgpd.svg
```

## Opções de Implantação

### 1. GitHub Pages

GitHub Pages é uma solução gratuita para hospedar sites estáticos diretamente de um repositório GitHub.

#### Passos para implantação:

1. **Crie uma conta no GitHub** (se ainda não tiver uma) em [github.com](https://github.com/)

2. **Crie um novo repositório**:
   - Acesse seu perfil e clique em "New repository"
   - Nomeie o repositório (ex: "fonotech-site")
   - Deixe-o público
   - Clique em "Create repository"

3. **Faça upload dos arquivos**:
   - Na página do repositório, clique em "Add file" > "Upload files"
   - Arraste todos os arquivos e pastas do projeto ou use o seletor de arquivos
   - Adicione uma mensagem de commit como "Primeira versão do site"
   - Clique em "Commit changes"

4. **Ative o GitHub Pages**:
   - Vá para "Settings" > "Pages"
   - Em "Source", selecione "main" (ou "master") branch
   - Clique em "Save"
   - Aguarde alguns minutos para o site ser publicado

5. **Acesse seu site**:
   - O URL será algo como `https://seu-usuario.github.io/fonotech-site/`
   - Este link aparecerá na seção GitHub Pages das configurações

### 2. Netlify

Netlify oferece hospedagem gratuita com recursos adicionais como formulários funcionais.

#### Passos para implantação:

1. **Crie uma conta no Netlify** em [netlify.com](https://www.netlify.com/) (pode usar sua conta GitHub para login)

2. **Implante o site**:
   - Na dashboard do Netlify, clique em "Add new site" > "Deploy manually"
   - Arraste a pasta do projeto inteira para a área indicada
   - Aguarde o upload e processamento

3. **Configure seu site**:
   - Após o deploy, clique em "Site settings"
   - Em "Site details", você pode alterar o nome do site (URL)
   - O URL padrão será algo como `https://random-name.netlify.app`

4. **Ative o formulário** (opcional):
   - No arquivo `index.html`, adicione o atributo `data-netlify="true"` à tag `<form>`
   - Reimplante o site para ativar a funcionalidade de formulário

### 3. Vercel

Vercel é outra excelente opção gratuita para sites estáticos.

#### Passos para implantação:

1. **Crie uma conta no Vercel** em [vercel.com](https://vercel.com/) (pode usar sua conta GitHub)

2. **Implante o site**:
   - Na dashboard, clique em "New Project" > "Upload"
   - Arraste a pasta do projeto ou selecione os arquivos
   - Clique em "Deploy"

3. **Configure seu site**:
   - Após o deploy, você pode personalizar o domínio nas configurações do projeto
   - O URL padrão será algo como `https://fonotech-site.vercel.app`

### 4. Cloudflare Pages

Cloudflare Pages oferece hospedagem gratuita com CDN global.

#### Passos para implantação:

1. **Crie uma conta no Cloudflare** em [cloudflare.com](https://www.cloudflare.com/)

2. **Acesse Cloudflare Pages**:
   - No painel, vá para "Pages"
   - Clique em "Create a project" > "Direct upload"

3. **Faça upload do site**:
   - Dê um nome ao projeto (ex: "fonotech-site")
   - Arraste a pasta do projeto ou selecione os arquivos
   - Clique em "Deploy site"

4. **Acesse seu site**:
   - O URL será algo como `https://fonotech-site.pages.dev`

## Personalização do Site

Para personalizar o site antes da implantação:

1. **Substituir imagens placeholder**:
   - Substitua os arquivos SVG na pasta `images/` por imagens reais relacionadas ao tema
   - Mantenha os mesmos nomes de arquivo para evitar quebrar os links

2. **Personalizar cores**:
   - Edite as variáveis CSS no início do arquivo `css/styles.css`
   - Altere as cores primárias, secundárias e de destaque conforme necessário

3. **Configurar formulário**:
   - Para formulários funcionais, considere usar serviços como:
     - Formspree (gratuito): Adicione `action="https://formspree.io/f/seu-id"` à tag `<form>`
     - Netlify Forms: Adicione `data-netlify="true"` à tag `<form>` (se hospedar no Netlify)

## Considerações Finais

- Este é um site estático, então o formulário precisará de um serviço externo para processamento
- Para adicionar um domínio personalizado, consulte a documentação da plataforma escolhida
- Recomenda-se testar o site em diferentes dispositivos e navegadores antes da implantação final

Para qualquer dúvida adicional sobre a implantação, consulte a documentação oficial da plataforma escolhida.
