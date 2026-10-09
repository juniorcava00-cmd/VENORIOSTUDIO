# VEORIO STUDIO — site local

Site estático, responsivo e pronto para abrir no navegador. Para habilitar instalação e uso offline, sirva esta pasta por HTTP ou HTTPS. Em desenvolvimento, execute py -m http.server 8000 nesta pasta e abra http://localhost:8000.

## Tecnologias

- HTML semântico, CSS responsivo e JavaScript nativo.
- Bootstrap 5.3.8 mantido localmente para a grade dos estudos de portfólio.
- Fontes Inter e Archivo auto-hospedadas, com licenças OFL incluídas.
- Progressive Web App com manifesto e cache offline por service worker.
- Formulário de briefing preparado localmente; não envia nem armazena dados nesta versão.
- Sem CDN, API ou serviço externo obrigatório.

A direção visual combina uma base editorial branca, cinza e preta com azul cobalto vivo (#2458f5) em botões, títulos, links, interações e detalhes gráficos. Sem tons laranja. O site preserva os serviços e os quatro estudos conceituais, claramente identificados como demonstrações.

## Contato

Antes de divulgar, preencha os canais reais em window.VEORIO_CONFIG no fim de index.html:

    window.VEORIO_CONFIG = {
      whatsapp: "5511999999999",
      email: "contato@seudominio.com.br",
      instagram: "https://instagram.com/seuperfil"
    };

Sem contato configurado, o formulário prepara a solicitação e explica que ela não foi enviada. Os quatro itens de portfólio são estudos conceituais, não trabalhos de clientes.
