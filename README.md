# DESTAKWEB - Website Institucional Premium & Tecnológico

Website completo, leve, responsivo e de alta performance desenvolvido com arquitetura estática pura (**HTML5 semântico, CSS3 moderno e JavaScript Vanilla**).

---

## 🚀 Como Hospedar em Qualquer Servidor

Como o projeto não depende de Node.js, compilações ou banco de dados no frontend, você pode publicá-lo em **qualquer provedor de hospedagem** apenas enviando os arquivos:

### 1. Hospedagens Tradicionais (cPanel, Hostinger, KingHost, Locaweb, Apache, NGINX):
- Acesse o gerenciador de arquivos ou FTP da sua hospedagem.
- Envie todo o conteúdo da pasta `c:/DESTAKWEB/` para dentro do diretório raiz do seu domínio (geralmente chamado de `public_html` ou `www`).
- Pronto! O site já estará no ar.

### 2. Hospedagens Gratuitas / Nuvem (Vercel, Netlify, GitHub Pages):
- **Vercel / Netlify**: Basta arrastar a pasta `DESTAKWEB` para o painel ou conectar com um repositório GitHub.
- **GitHub Pages**: Suba os arquivos para um repositório e ative o *GitHub Pages* nas configurações.

---

## ⚙️ Como Personalizar

### 1. Alterar o Número do WhatsApp
Para receber as propostas da calculadora diretamente no seu número do WhatsApp:
1. Abra o arquivo `js/calculator.js`.
2. Na linha 8, altere o valor de `phone`:
   ```javascript
   const WHATSAPP_CONFIG = {
     phone: '5511999999999', // Substitua pelo seu DDI + DDD + Número sem espaços nem traços
   ```
3. No arquivo `index.html`, procure pelo link do botão flutuante de WhatsApp e atualize o número `5511999999999` para o seu.

### 2. Configurar o Canal do Telegram
No arquivo `index.html`, procure por `https://t.me/seucanaltelegram` e substitua pelo link ou username oficial do seu canal no Telegram (ex: `https://t.me/destakweb`).

### 3. Inserir a Logomarca da Empresa
Quando quiser aplicar a imagem oficial da sua marca:
1. Salve o arquivo da sua logo com o nome `logo.png` ou `logo.svg` dentro da pasta `assets/images/` (ou seja: `c:/DESTAKWEB/assets/images/logo.png`).
2. O site já está programado para carregar automaticamente a imagem no cabeçalho e rodapé mantendo a proporção perfeita!

### 4. Alterar Preços ou Serviços do Simulador
No arquivo `js/calculator.js`, o objeto `SERVICES_DATA` contém todos os preços base, nomes e adicionais para:
- **Desenvolvimento Web** (`web`)
- **Manutenção de Notebooks & PCs** (`maint`)
- **Retrô Games** (`retro`)
- **Nuvem & Backup Local** (`cloud`)

Basta alterar os valores numéricos (`basePrice`, `price`) ou textos conforme sua tabela comercial.

---

## 📁 Estrutura de Arquivos

```
DESTAKWEB/
├── index.html          # Estrutura HTML semântica com todas as seções
├── css/
│   ├── style.css       # Design System, variáveis de cores, hero, layout geral
│   ├── components.css  # Botões, modais, formulários, badges e efeitos
│   └── responsive.css  # Ajustes para Mobile, Tablets e Desktops
├── js/
│   ├── main.js         # Menu mobile, rolagem suave, indicador de menu e modais
│   └── calculator.js   # Simulador interativo com cálculo dinâmico e integração WhatsApp
└── README.md           # Guia de uso e publicação
```
