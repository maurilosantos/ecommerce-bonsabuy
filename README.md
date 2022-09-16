# E-commerce: Bonsabuy
## Índice
<!--ts-->
* [Descrição do Projeto](#descrição-do-projeto-)
* [Função](#função-)
* [Tecnologias Utilizadas](#tecnologias-utilizadas-)
* [Como acessar](#como-acessar-)
* [Conhecimentos Bootstrap](#conhecimentos-bootstrap-)
* [Autor](#autor-)
<!--te-->
<img src="https://img.shields.io/badge/status-completo-green"><br>

# Descrição do projeto <br>
Uma landing page de E-commerce utilizando e compartilhando conhecimentos em Bootstrap. Na página basciamente existe o NavBar e Cards para confecção dos produtos.<br><br>

# Função <br>
![mobile (3)](https://user-images.githubusercontent.com/109925535/190789993-0839c930-df72-48d3-8cd7-3435a7047f59.gif)


# Tecnologias Utilizadas <br>
Bootstrap, GIT. </br>


# Como acessar <br>
<a href="https://maurilosantos.github.io/ecommerce-bonsabuy/">Acesse aqui</a>

# Conhecimentos Bootstrap <br>
Tópicos estudados através da <a href="https://getbootstrap.com.br/docs/4.1/getting-started/introduction/">documentação </a>:<br>
- **Cores**
    
    ```html
    <p class="text-primary">.text-primary</p>
    <p class="text-secondary">.text-secondary</p>
    <p class="text-success">.text-success</p>
    <p class="text-danger">.text-danger</p>
    <p class="text-warning">.text-warning</p>
    <p class="text-info">.text-info</p>
    <p class="text-light bg-dark">.text-light</p>
    <p class="text-dark">.text-dark</p>
    <p class="text-body">.text-body</p>
    <p class="text-muted">.text-muted</p>
    <p class="text-white bg-dark">.text-white</p>
    <p class="text-black-50">.text-black-50</p>
    <p class="text-white-50 bg-dark">.text-white-50</p>
    ```
    
- **Display**
    - `d-{valor}` para o breakpoint `xs`;
    - `d-{breakpoint}-{valor}` para os breakpoints `sm`, `md`, `lg` e `xl`.
    
    Onde a parte *{valor}* deve ser substituída por:
    
    - `none`;
    - `inline`;
    - `inline-block`;
    - `block`;
    - `table`;
    - `table-cell`;
    - `table-row`;
    - `flex`;
    - `inline-flex`.
    
    As media queries afetam as laguras das telas com o dado ou maior breakpoint. Por exemplo, `.d-lg-none` define `display: none;` tanto em telas de tamanho `lg`, quanto `xl`.
    
- **Margin e Padding**
    
    Use os [utilitários de espaçamento](https://getbootstrap.com.br/docs/4.1/utilities/spacing/) de `margin` e `padding` para controlar como elementos e componentes são espaçados e dimensionados. Bootstrap 4 possui uma escala de cinco níveis para utilitários de espaçamento, baseado no valor padrão `1rem` da variável `$spacer`. Escolha valores para todas viewports (`.mr-3`, no caso `margin-right: 1rem`) ou variações responsivas para mirar em viewports específicas (`.mr-md-3` para `margin-right: 1rem` em viewports do breakpoint `md`).
    
    O campo *propriedade* pode ser:
    
    - `m` - para usar `margin`;
    - `p` - para usar `padding`.
    
    O campo *lados* pode ser:
    
    - `t` - para usar `margin-top` ou `padding-top`;
    - `b` - para usar `margin-bottom` ou `padding-bottom`;
    - `l` - para usar `margin-left` ou `padding-left`;
    - `r` - para usar `margin-right` ou `padding-right`;
    - `x` - para usar margem ou padding, tanto na esquerda quanto direita;
    - `y` - para usar margem ou padding, tanto na parte superior quanto na inferior;
    - Deixe o campo em branco, para usar `margin` ou `padding` em todos os quatro lados do elemento.
    
    O campo *tamanho* pode ser:
    
    - `0` - para remover o `padding` ou `margin`;
    - `1` - para usar a `margin` ou `padding` com valor de `$spacer * .25`;
    - `2` - para usar a `margin` ou `padding` com valor de `$spacer * .5`;
    - `3` - para usar a `margin` ou `padding` com valor de `$spacer`;
    - `4` - para usar a `margin` ou `padding` com valor de `$spacer * 1.5`;
    - `5` - para usar a `margin` ou `padding` com valor de `$spacer * 3`;
    - `auto` - para usar a `margin` com valor de `auto`.
    
    *Ps: você pode adicionar mais tamanhos, colocando mais valores no mapa Sass `$spacers`.*
    
- **Container**
    
    Containers são os elementos de layout mais básico do Bootstrap e são **necessários quando usamos o sistema de grid padrão**. 
    Escolha entre um container responsivo de largura fixa (ou seja, com alterações de `max-width` em cada ponto de interrupção) ou por um responsivo de largura fluida (ou seja, `100%` de largura o tempo todo).
    
    ```html
    <div class="container">
      <!-- Conteúdo aqui -->
    </div>
    ```
    
    Ou essa que abrange toda área da vizualização:
    
    ```html
    <div class="container-fluid">
      ...
    </div>
    ```
    
- **Responsividade**
    
    Temos quatro elementos no bootstrap que ditam a responsividade: 
    
    `sm`:  aplicando em telas ≥ 576 px
    
    `md`: aplicado em telas ≥ 768 px
    
    `lg`:  aplicado em telas ≥ 992 px
    
    `xl`:  aplicado em telas ≥ 1200 px
    
    ```html
    <div class="float-sm-left">Flutua à esquerda, em viewports de tamanho SM (pequena) ou maior.</div><br>
    <div class="float-md-left">Flutua à esquerda, em viewports de tamanho MD (média) ou maior.</div><br>
    <div class="float-lg-left">Flutua à esquerda, em viewports de tamanho LG (grande) ou maior.</div><br>
    <div class="float-xl-left">Flutua à esquerda, em viewports de tamanho XL (extra-grande) ou maior.</div><br>
    ```
    
- **Flexbox**
    
    ```html
    <div class="d-flex p-2 bd-highlight">Eu sou um flex container!</div>
    ```
    
    Variações responsivas também existem para `.d-flex` e `.d-inline-flex`.
    
    - `.d-flex`
    - `.d-inline-flex`
    - `.d-sm-flex`
    - `.d-sm-inline-flex`
    - `.d-md-flex`
    - `.d-md-inline-flex`
    - `.d-lg-flex`
    - `.d-lg-inline-flex`
    - `.d-xl-flex`
    - `.d-xl-inline-flex`
    
    [Mais informações](https://getbootstrap.com.br/docs/4.1/utilities/flex/)
    
- **Grid**
    
    O sistema grid Bootstrap usa vários containers, linhas e colunas para arranjar e alinhar conteúdo. Ele é feito com [flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox) e é, totalmente, responsivo.
    
    ```html
    <div class="container">
      <div class="row">
        <div class="col-sm">
          Uma de três colunas
        </div>
        <div class="col-sm">
          Uma de três colunas
        </div>
        <div class="col-sm">
          Uma de três colunas
        </div>
      </div>
    </div>
    ```
    
    O exemplo acima cria três colunas de larguras idênticas em dispositivos pequenos, médios, grandes e extra grandes, usando nossas classes grid pré-definidas. Estas colunas são centralizadas na página, usando o elemento pai `.container`.
    
    Resumindo, assim é como funciona:
    
    - Containers criam meios para centralizar e, horizontalmente, preencher os conteúdos de seu site;
        - Use `.container` para ter uma largura responsiva em pixel ou `.container-fluid` para ter `width: 100%`, em todas viewports e tamanhos de disposivos.
    - Rows são elemntos para envolver colunas;
        - Cada coluna tem `padding` horizontal (gutter) para controlar o espaço, entre elas.
            - Este `padding`, depois, é cancelado com rows usando margens negativas. Assim, todo conteúdo em suas colunas é, visualmente, alinhado a esquerda.
    - Em um layout grid, o conteúdo deve ser posicionado dentro de colunas e só elas podem ser filhos imediatos de `.row`s;
    - Graças ao flexbox, colunas grid sem `width` declarado vão, automaticamente, se dimensionar com larguras iguais;
        - Por exemplo, quatro exemplos de `.col-sm` vão, automaticamente, ter 25% de largura, no breakpoint `sm` ou maior;
        - Veja a seção [colunas com layout automático](https://getbootstrap.com.br/docs/4.1/layout/grid/#auto-layout-columns), para mais exemplos.
    - Classes de colunas indicam o número de colunas que você quer usar, dentro de uma possibilidade de 12, por row;
        - Se você quiser três colunas de larguras idênticas, pode usar `.col-4`, por exemplo.
    - Largura de colunas são definidas em porcentagem para que, então, elas sejam sempre fluidas e dimensionadas com relação a seus elementos pais;
    - Colunas possuem `padding` horizontal para criar gutters, entre cada coluna.
        - No entanto, você pode remover a `margin` das rows e `padding` das colunas, usando `.no-gutters` na `.row`.
    - Para fazer o grid responsivo, existem cinco breakpoints, um para cada [breakpoint responsivo](https://getbootstrap.com.br/docs/4.1/layout/overview/#responsive-breakpoints): extra small (implícito), small, medium, large e extra large;
    - Breakpoints grid são baseados em media queries `min-width`, significando que **elas aplicam estilos para o dado breakpoint e outros maiores**;
        - Exemplo: `.col-sm-4` aplica ao small, medium, large e extra large, mas não ao primeiro breakpoint `xs`.
    - Você pode usar classes grid pré-definidas (como `.col-4`) ou [mixins Sass](https://getbootstrap.com.br/docs/4.1/layout/grid/#sass-mixins) com uma marcação mais semântica.
    
    Se atente as limitações e [bugs flexbox](https://github.com/philipwalton/flexbugs), tipo a [impossibilidade de usar alguns elementos HTML como container flex](https://github.com/philipwalton/flexbugs#flexbug-9).
    
- **Tipografia**
    
    ### Tipografia
    
    [Documentação](https://getbootstrap.com.br/docs/4.1/content/typography/) e exemplos para a tipografia Bootstrap, incluindo configurações globais, cabeçalhos, listas, texto do `<body>` e outros.
    
- **Imagens**
    
    [Documentação](https://getbootstrap.com.br/docs/4.1/content/images/)
    
- **Tabelas**
    
    Devido ao abrangente uso de tabelas em *widgets* de terceiros, como calendários e selecionadores da datas, nós desenvolvemos nossas tabelas de forma que sejam **alternativas**. Basta adicionar a classe `.table` em qualquer `<table>`, então, customize-a mais usando nossos estilos de costumização ou as diversas classes modificadoras. Veja a [documentação](https://getbootstrap.com.br/docs/4.1/content/tables/).
    
- **Alerts**
    
    Alertas estão disponíveis para qualquer tamanho de texto, assim como um botão de dispersão opcional. Para uma estilização adequada, use uma das oito **requeridas** classes contextuais (ex: `.alert-success`). Para dispersão inline, use o plugin [jQuery alerts](https://getbootstrap.com.br/docs/4.1/components/alerts/#dismissing). Veja a [documentação](https://getbootstrap.com.br/docs/4.1/components/alerts/).
    
- **Botões**
    
    [Documentação](https://getbootstrap.com.br/docs/4.1/components/buttons/)
    
- **Collapse**
    
    O plugin JavaScript collapse é usado para mostrar e esconder conteúdo. Botões ou âncoras são usados como gatilhos que são mapeados para elementos específicos que você alterna visibilidade. Mostrar um elemento (de tal maneira) vai animar a `height`, de seu valor atual, para `0`. Dado como CSS lida com animações, você não pode usar `padding` em um elemento `.collapse`. Pelo contrário, use esta classe como um elemento pai independente. [Documentação](https://getbootstrap.com.br/docs/4.1/components/collapse/).****
    
- **DropDown**
    
    Dropdowns são botões com alternância de visibilidade de listas de links e outras coisas. Conseguem ser interativos graças a sua construção que foi feita com o plugin JavaScript dropdown. [Documentação](https://getbootstrap.com.br/docs/4.1/components/dropdowns/).
    
- **Cards**
    
    Um **card** é um container de conteúdo flexível e extensível. Ele tem opções para cabeçalhos e rodapés, uma larga variedade de conteúdo, cores de background contextuais e opções de display poderosas. Se você é familiarizado com Bootstrap 3, saiba que os cards substituem nossos antigos panels, wells e thumbnails. Uma funcionalidade similar a destes componentes está disponível, usando classes modificadoras para cards. [Documentação](https://getbootstrap.com.br/docs/4.1/components/card/).****
    
- **Progress**
    
    Componentes de progresso são feitos com dois elementos HTML, um pouco de CSS para a largura e outros atributos. Não usamos [o elemento HTML5 `<progress>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/progress) para garantir que você possa empilhar barras de progresso e colocar textos sobre elas. [Documentação](https://getbootstrap.com.br/docs/4.1/components/progress/).
    
- **Grupo de lista**
    
    Grupos de listas são componentes flexíveis e poderosos para mostrar vários conteúdos. Modifique e aprimore-o para suportar quase qualquer conteúdo. [Documentação](https://getbootstrap.com.br/docs/4.1/components/list-group/).****
    
- **Paginação**
    
    Documentação e exemplos de paginação para indicar um série de conteúdos relacionados, existentes em várias páginas. [Documentação](https://getbootstrap.com.br/docs/4.1/components/pagination/).****
    
- **Nav**
    
    A navegação disponível no Bootstrap compartilha várias marcações e estilos, desde a classe base `.nav` até os estados ativo e desativo. [Documentação](https://getbootstrap.com.br/docs/4.1/components/navs/).
    
- **Navbar**
    
    Documentação e exemplos para o poderoso e responsivo cabeçalho de navegação, o navbar. Inclui suporte para logo, navegação, plugin collapse e muito mais. [Documentação](https://getbootstrap.com.br/docs/4.1/components/navbar/).****
    
- **Carousel**
    
    Um componente de slideshow para fazer um giro através de elementos (imagens ou slides de texto), como se fosse um carrosel. **Documentação**.****
    
- **Modal**
    
    Use o plugin JavaScript modal para criar diálogos em seu site para notificações e outros tipos de conteúdos customizados. [Documentação](https://getbootstrap.com.br/docs/4.1/components/modal/).****
    
- **Tootips**
    
    [Documentação](https://getbootstrap.com.br/docs/4.1/components/tooltips/) e exemplos para criar tooltips Bootstrap personalizados com CSS e JavaScript, usando CSS3 para animações e atributos data para armazenamento local de título. ****
    
- **Popovers**
    
    Coisas para saber, quando usando o plugin popover:
    
    - O popover depende da biblioteca externa [Popper.js](https://popper.js.org/), para posicionamento. Você deve colocar [popper.min.js](https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js) antes de `bootstrap.js` ou usar `bootstrap.bundle.min.js` / `bootstrap.bundle.js`, os quais contém Popper.js para o popover funcionar.
    - Popovers precisam do [plugin tooltip](https://getbootstrap.com.br/docs/4.1/components/tooltips/), como sua dependência;
    - Se você está montando o JavaScript a partir da fonte, vai precisar do `[util.js](https://getbootstrap.com.br/docs/4.1/getting-started/javascript/#util)`;
    - Popovers são opcionais por motivos de desempenho, então, **você deve inciá-lo, por conta própria**;
    - Atributos `title` e `content` vazios nunca vão ser mostrados em um popover;
    - Declare `container: 'body'` para evitar problemas de renderização, em componentes mais complexos (como nos grupos de inputs ou botões);
    - Acionar popovers em elementos ocultos não funciona;
    - Popovers em elementos `.disabled` ou `disabled` devem ser acionados em um elemento pai;
    - Quando acionados por âncoras que envolvem várias linhas, os popovers serão centralizados entre a largura total das âncoras. Use `white-space: nowrap;` em seus `<a>`, para evitar este comportamento.
    - Popovers devem ser ocultos, antes que seus elementos correspondentes sejam removidos do DOM.
# Autor <br>

[<img src="https://avatars.githubusercontent.com/u/109925535?v=4" width=115><br><sub>Maurilo Santos</sub>](https://github.com/maurilosantos) 



