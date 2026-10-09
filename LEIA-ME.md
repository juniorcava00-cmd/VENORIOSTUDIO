# VEORIO STUDIO — site local

Sirva esta pasta por HTTP ou HTTPS para conferir o site e habilitar o PWA. O service worker e a instalação como app não funcionam quando `index.html` é aberto diretamente como arquivo. Em desenvolvimento, use `py -m http.server 8000` nesta pasta e abra `http://localhost:8000`.

O site é estático e não depende de bibliotecas externas. Inclui layout responsivo, navegação por teclado, estudos de portfólio identificados como conceitos, filtros, perguntas frequentes, formulário de briefing, metadados de compartilhamento e suporte PWA. Após a primeira visita online, o shell e os arquivos locais ficam disponíveis offline. O navegador oferece a instalação quando o dispositivo é compatível.

## Tecnologias

- Bootstrap 5.3.8 local para as colunas responsivas do portfólio.
- Inter e Archivo auto-hospedadas; as licenças OFL estão em `assets/fonts`.
- JavaScript nativo para navegação, filtros, diálogo, animações e formulário; IntersectionObserver respeita a preferência de movimento reduzido.
- Service worker e manifesto PWA para instalação e cache offline.

A composição visual foi refeita com apresentação fotográfica em tela cheia, seções alternadas claras e escuras, navegação compacta e projetos em destaque. Os textos e os estudos conceituais do VEORIO foram mantidos.

A página Titan de referência entrega Bootstrap 4.6.2 e jQuery 3.7.1. O VEORIO usa a versão atual do Bootstrap 5, que não precisa de jQuery, e mantém os arquivos no pacote para funcionar sem CDN.

## Contato

Antes de divulgar o site, preencha os canais de contato reais em `window.VEORIO_CONFIG`, antes do script principal no fim de `index.html`:

```html
<script>
  window.VEORIO_CONFIG = {
    whatsapp: "5511999999999",
    email: "contato@seudominio.com.br",
    instagram: "https://instagram.com/seuperfil"
  };
</script>
```

Use o número de WhatsApp com código do país e DDD, somente com dígitos. Sem WhatsApp ou e-mail reais, o formulário prepara a mensagem e explica que ela não foi enviada. Ele não armazena nem transmite os dados; com um canal configurado, abre o WhatsApp ou o aplicativo de e-mail do visitante.

Os quatro itens do portfólio são estudos conceituais demonstrativos, não trabalhos de clientes.
