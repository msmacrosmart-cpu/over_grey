# Over Grey — Noodle & Co

**Noodle & Co — Udon Artesanal**

Landing page de restaurante de macarrão udon, com tema escuro e dourado:
cardápio de pratos, opções de combos, horário de funcionamento e contato.

## 🚀 Como rodar

O site usa módulos ES, então **abrir com duplo clique (`file://`) não funciona** —
é preciso servir por HTTP:

```bash
python3 -m http.server 8000
# acesse http://localhost:8000
```

## 📁 Estrutura

```
.
├── index.html   # aplicação completa (HTML + CSS + JS empacotados)
├── images/      # 7 fotos usadas no site (~1,8 MB)
│   ├── bg-texture.jpg             # textura de fundo (via CSS)
│   ├── udon-carne-grelhada.jpg
│   ├── udon-molho-porco.jpg
│   ├── udon-classico-ovo.jpg
│   ├── combo-refrigerante.jpg
│   ├── combo-suco.jpg
│   └── combo-bebida.jpg
└── README.md
```

## 🛠️ Tecnologias

- React (aplicação de página única)
- Build empacotado com Vite, com CSS e JS inline
- Google Fonts — Playfair Display e Inter
- Imagens locais na pasta `images/`

## 🌐 GitHub Pages

Para publicar gratuitamente:

1. Vá em **Settings → Pages**
2. Em *Source*, selecione a branch `main` e a pasta `/ (root)`
3. Salve — o site ficará disponível em
   `https://msmacrosmart-cpu.github.io/over_grey/`

Os caminhos das imagens são **relativos** (`images/...`), então funcionam
tanto na raiz de um domínio quanto em um subcaminho de projeto do Pages.

## ⚠️ Observação sobre prints e prévias

Por ser uma aplicação React, o conteúdo é renderizado por JavaScript.
Serviços de screenshot e cartões de prévia (Microlink, WhatsApp, LinkedIn)
que não executam JS podem capturar uma página em branco. Nesse caso é
preciso gerar uma versão pré-renderizada (HTML estático) do site.

## 📄 Licença

Projeto de uso pessoal/demonstrativo.
