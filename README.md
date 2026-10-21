# DevClub Store

Uma vitrine de produtos com tema futurista, feita com HTML, CSS e JavaScript puro. A página apresenta três produtos em um carrossel com transições animadas, controles de navegação e indicadores de posição.

## Funcionalidades

- Exibe três produtos: Apple Watch Series 10, AirPods Max e Vision Pro.
- Avança automaticamente para o próximo produto a cada 5 segundos.
- Permite navegar entre os produtos usando os botões de anterior e próximo.
- Mostra o número e o indicador visual do produto atual.
- Anima a entrada e a saída dos produtos, incluindo imagens, textos e botões.
- Usa um fundo em gradiente, círculos decorativos e um efeito pulsante de luz.
- Carrega as fontes Montserrat e Orbitron pelo Google Fonts.

## Tecnologias

- **HTML5** para a estrutura da página.
- **CSS3** para o layout, os efeitos visuais e as animações.
- **JavaScript** para o carrossel, a navegação e a troca automática de produtos.

O projeto não utiliza frameworks nem dependências de JavaScript.

## Estrutura dos arquivos

```text
Devclub Store/
├── index.html
├── styles.css
├── scripts.js
└── img/
    ├── air-pods.png
    ├── apple-watch.png
    └── vision-pro.png
```

- `index.html`: conteúdo e estrutura da vitrine.
- `styles.css`: estilos, layout responsivo do conteúdo existente e animações.
- `scripts.js`: lógica de navegação e atualização do carrossel.
- `img/`: imagens dos produtos exibidos.

## Como executar

1. Baixe ou clone os arquivos do projeto.
2. Abra `index.html` em um navegador.

Não é necessário instalar pacotes ou iniciar um servidor para visualizar a página. É necessária uma conexão com a internet para carregar as fontes do Google Fonts.

## Como funciona o carrossel

Os produtos ficam em elementos com a classe `.item`. O produto visível recebe também a classe `.active`; o JavaScript alterna essa classe ao navegar. O CSS usa as classes para controlar a opacidade e a posição dos elementos, criando as transições.

Os botões com os IDs `prev` e `next` alteram o produto atual. O script também avança automaticamente a cada 5 segundos. Os elementos `.dot` e `.numbers` acompanham a posição atual.

## Personalização

- **Adicionar ou editar produtos:** altere os elementos `.item` em `index.html`, incluindo a imagem, o texto e o botão.
- **Trocar imagens:** coloque os arquivos em `img/` e atualize o atributo `src` da imagem correspondente.
- **Mudar cores, espaçamentos ou animações:** edite as regras em `styles.css`.
- **Alterar o intervalo automático:** ajuste o valor `5000` usado em `setInterval` em `scripts.js`. O valor está em milissegundos.

Se adicionar ou remover produtos, mantenha a mesma quantidade de elementos `.dot` dos elementos `.item`, pois os indicadores são atualizados pelo JavaScript pela posição correspondente.
