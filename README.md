<h1><strong>Desafio Técnico. Manipulação de DOM</strong></h1>

<h2><strong>Descrição</strong></h2>
<p align="justify">
  Este repositório contém a resolução do exercício <strong>Desafio Técnico. Manipulação de DOM</strong>, baseado no desafio da Trybe.
  A proposta é simular um teste técnico para uma vaga de emprego, em que o objetivo é demonstrar habilidades em
  <strong>manipulação do DOM com JavaScript puro</strong>, alterando elementos de uma página HTML já existente.
</p>
<p align="justify">
  O projeto parte de um código inicial parcialmente implementado. A partir dele, foram realizadas modificações definidas nos
  <strong>Requisitos do Projeto</strong>, utilizando apenas as funções nativas de seleção do DOM:
  <code>document.getElementById()</code>, <code>document.getElementsByClassName()</code> e
  <code>document.getElementsByTagName()</code>.
</p>

<h2><strong>Contexto do Exercício</strong></h2>
<p align="justify">
  Boas vindas ao exercício <strong>Desafio Técnico. Manipulação de DOM</strong>.
  É hora de aplicar conhecimentos em manipular elementos do HTML, simulando um desafio real de processo seletivo.
</p>
<ul>
  <li align="justify">
    Imagine que você recebeu um desafio técnico para uma vaga, em que precisa mostrar sua capacidade de manipular o DOM.
  </li>
  <li align="justify">
    O projeto já vem parcialmente pronto, e as alterações que devem ser feitas estão descritas nos requisitos.
  </li>
  <li align="justify">
    Ao iniciar o exercício, você concorda com o Código de Conduta e com o Manual da Pessoa Estudante da Trybe.
  </li>
</ul>

<h2><strong>Tecnologias Utilizadas</strong></h2>
<ul>
  <li align="justify">
    <a href="https://developer.mozilla.org/pt-BR/docs/Web/HTML" target="_blank"><strong>HTML5</strong></a>. 
    Estrutura da página e marcação dos elementos que serão manipulados via JavaScript.
  </li>
  <li align="justify">
    <a href="https://developer.mozilla.org/pt-BR/docs/Web/CSS" target="_blank"><strong>CSS3</strong></a>. 
    Estilização base da página, definição de cores de fundo, bordas e layout.
  </li>
  <li align="justify">
    <a href="https://developer.mozilla.org/pt-BR/docs/Web/JavaScript" target="_blank"><strong>JavaScript</strong></a>. 
    Manipulação de DOM, alteração de textos, estilos e seleção de elementos usando apenas
    <code>getElementById</code>, <code>getElementsByClassName</code> e <code>getElementsByTagName</code>.
  </li>
  <li align="justify">
    <a href="https://www.cypress.io/" target="_blank"><strong>Cypress</strong></a>. 
    Ferramenta de testes automatizados utilizada pela Trybe para validar o comportamento esperado das soluções.
  </li>
</ul>

<h2><strong>Estrutura do Projeto</strong></h2>
<p align="justify">A estrutura de arquivos do projeto é organizada da seguinte forma.</p>

<pre>
dom-manipulation/
├── cypress/               Arquivos de testes automatizados
├── images/                Imagens de apoio ao exercício
├── .editorconfig          Configurações de formatação de código
├── .eslintrc.json         Regras de lint para JavaScript
├── .gitignore             Arquivos e pastas ignorados pelo Git
├── .stylelintrc.json      Regras de lint para CSS
├── README.md              Documentação do exercício
├── cypress.json           Configurações do Cypress
├── index.html             Estrutura HTML base fornecida pela Trybe
├── package-lock.json      Detalhamento das dependências instaladas
├── package.json           Dependências e scripts npm
├── reporter.json          Relatórios de testes
└── style.css              Estilos principais da página
</pre>

<h2><strong>HTML Base do Desafio</strong></h2>
<p align="justify">
  O desafio começa a partir do seguinte trecho de HTML base, que não deve ser alterado diretamente.
  As modificações devem ser feitas via JavaScript, dentro da tag <code>&lt;script&gt;</code>.
</p>

<pre>
&lt;!DOCTYPE html&gt;
&lt;html&gt;
  &lt;head&gt;
    &lt;meta charset="UTF-8" /&gt;
    &lt;meta name="viewport" content="width=device-width" /&gt;
    &lt;title&gt;Exercício&lt;/title&gt;
    &lt;style&gt;
      main, section {
        border-color: black;
        border-style: solid;
      }

      .title {
        text-align: center;
      }

      .main-content {
        background-color: yellow;
      }

      .main-content .center-content {
        background-color: red;
        width: 50%;
        margin: 0 auto;
      }

      .main-content .center-content p {
        font-style: italic;
      }
    &lt;/style&gt;
  &lt;/head&gt;
  &lt;body&gt;
    &lt;header&gt; 
      &lt;h1 class="title"&gt;Desafio - JavaEscripito&lt;/h1&gt;
    &lt;/header&gt;    
    &lt;main class="main-content"&gt;
      &lt;section class="center-content"&gt;
        &lt;p&gt;Texto padrão do nosso site&lt;/p&gt;
        &lt;p&gt;-----&lt;/p&gt;
        &lt;p&gt;Trybe&lt;/p&gt;
      &lt;/section&gt;
    &lt;/main&gt;
    &lt;p&gt;Último parágrafo.&lt;/p&gt;
    &lt;script&gt;
      // Seu código aqui
    &lt;/script&gt;
  &lt;/body&gt;
&lt;/html&gt;
</pre>

<h2><strong>Regras de Manipulação do DOM</strong></h2>
<p align="justify">
  Para avaliar o conhecimento em HTML e JavaScript, as alterações devem ser feitas apenas com as funções:
</p>
<ul>
  <li><code>document.getElementById()</code></li>
  <li><code>document.getElementsByClassName()</code></li>
  <li><code>document.getElementsByTagName()</code></li>
</ul>

<h2><strong>Requisitos do Exercício</strong></h2>

<h3><strong>Exercício 1. Alterando o texto</strong></h3>
<p align="justify">
  Criar e executar uma função que mude o texto da tag <code>&lt;p&gt;-----&lt;/p&gt;</code> para uma
  descrição de como eu me vejo daqui a dois anos.
</p>

<h3><strong>Exercício 2. Alterando a cor do elemento amarelo</strong></h3>
<p align="justify">
  Criar e executar uma função que mude a cor de fundo do elemento amarelo
  <code>.main-content</code> para <code>rgb(76, 164, 109)</code>.
</p>

<h3><strong>Exercício 3. Alterando a cor do elemento vermelho</strong></h3>
<p align="justify">
  Criar e executar uma função que mude a cor de fundo do elemento vermelho
  <code>.center-content</code> para <strong>branco</strong>.
</p>

<h3><strong>Exercício 4. Corrigindo o título</strong></h3>
<p align="justify">
  Criar e executar uma função que corrija o texto da tag <code>&lt;h1&gt;</code>, ajustando o título
  para refletir corretamente o desafio de manipulação de DOM.
</p>

<h3><strong>Exercício 5. Letras maiúsculas</strong></h3>
<p align="justify">
  Criar e executar uma função que modifique o texto do primeiro parágrafo
  <code>&lt;p&gt;Texto padrão do nosso site&lt;/p&gt;</code> para que todo o conteúdo seja exibido em letras maiúsculas.
</p>

<h3><strong>Exercício 6. Exibindo conteúdo das tags &lt;p&gt;</strong></h3>
<p align="justify">
  Criar e executar uma função que exiba o conteúdo de todas as tags <code>&lt;p&gt;</code> da seção principal,
  isto é, dentro do elemento com <code>class="center-content"</code>.
  Os conteúdos devem ser concatenados em uma string única, separados por espaços,
  e podem ser exibidos no console ou em outro elemento da página.
</p>

<h2><strong>Objetivos de Aprendizado</strong></h2>
<ul>
  <li align="justify">
    Praticar a seleção de elementos do DOM usando <code>id</code>, <code>className</code> e <code>tagName</code>.
  </li>
  <li align="justify">
    Modificar textos e estilos de elementos HTML utilizando apenas JavaScript.
  </li>
  <li align="justify">
    Compreender melhor a estrutura em árvore do DOM e como percorrê-la na prática.
  </li>
  <li align="justify">
    Organizar o código em funções pequenas, reutilizáveis e fáceis de ler.
  </li>
  <li align="justify">
    Se aproximar do formato de desafios técnicos usados em processos seletivos e em atividades da Trybe.
  </li>
</ul>

<h2><strong>Como Executar o Projeto</strong></h2>

<h3><strong>1. Executar no navegador</strong></h3>
<ol>
  <li>Clone este repositório ou faça o download dos arquivos.</li>
  <li>Abra o arquivo <code>index.html</code> diretamente em um navegador.</li>
  <li>Verifique visualmente as alterações realizadas nas cores, textos e título.</li>
  <li>Abra o console do navegador para conferir saídas de texto de funções que exibem conteúdo das tags <code>&lt;p&gt;</code>, se implementadas dessa forma.</li>
</ol>

<h3><strong>2. Executar os testes com Cypress</strong></h3>
<ol>
  <li>
    Certifique-se de ter o 
    <a href="https://nodejs.org/" target="_blank"><strong>Node.js</strong></a> instalado.
  </li>
  <li>No terminal, dentro da pasta do projeto, execute:
    <ul>
      <li><code>npm install</code> para instalar as dependências.</li>
      <li><code>npm test</code> para rodar a suíte de testes com Cypress em modo padrão.</li>
      <li><code>npm run cypress:open</code> para abrir a interface gráfica do Cypress.</li>
      <li><code>npm run cy:browser</code> para rodar os testes em modo headless no navegador configurado.</li>
    </ul>
  </li>
</ol>

<h2><strong>Status do Projeto</strong></h2>
<p align="justify">
  Exercício <strong>concluído</strong> como parte dos estudos de fundamentos de JavaScript e manipulação de DOM.
  O repositório pode ser revisitado no futuro para refatoração, adição de comentários e melhorias de organização de código.
</p>

<h2><strong>Contact</strong></h2>
<p>
  <strong>Willian Gonçalves</strong> |
  <a href="https://www.linkedin.com/in/williandpg/" target="_blank"><strong>LinkedIn</strong></a> |
  <a href="https://github.com/williandpg" target="_blank"><strong>Github</strong></a> |
  <a href="https://williandpg.github.io/" target="_blank"><strong>Portfólio</strong></a> |
  <a href="mailto:goncalves.wdp@outlook.com" target="_blank"><strong>Email</strong></a>
</p>

<h2><strong>Créditos</strong></h2>
<p align="justify">
  Este exercício foi desenvolvido com base no material e no template de projeto fornecido pela 
  <strong>Trybe</strong>, e é utilizado aqui para fins de estudo e prática de manipulação de DOM com JavaScript.
</p>

<hr>

<details>
  <summary><strong>English Version</strong></summary>

  <h1><strong>Technical Challenge. DOM Manipulation</strong></h1>

  <h2><strong>Description</strong></h2>
  <p align="justify">
    This repository contains the solution for the <strong>DOM Manipulation Technical Challenge</strong>, based on a Trybe exercise.
    The goal is to simulate a job style technical test and demonstrate skills in
    <strong>DOM manipulation with vanilla JavaScript</strong> by changing elements of an existing HTML page.
  </p>

  <p align="justify">
    The project starts from a partially implemented base code.
    All required changes are defined in the challenge requirements and must be implemented only through JavaScript,
    using the native DOM selection methods <code>getElementById</code>, <code>getElementsByClassName</code> and
    <code>getElementsByTagName</code>.
  </p>

  <h2><strong>Technologies Used</strong></h2>
  <ul>
    <li align="justify">
      <a href="https://developer.mozilla.org/en-US/docs/Web/HTML" target="_blank"><strong>HTML5</strong></a>. 
      Base structure of the page and semantic markup for DOM manipulation.
    </li>
    <li align="justify">
      <a href="https://developer.mozilla.org/en-US/docs/Web/CSS" target="_blank"><strong>CSS3</strong></a>. 
      Initial styling, background colors, borders and simple layout.
    </li>
    <li align="justify">
      <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank"><strong>JavaScript</strong></a>. 
      DOM manipulation using <code>getElementById</code>, <code>getElementsByClassName</code> and
      <code>getElementsByTagName</code>.
    </li>
    <li align="justify">
      <a href="https://www.cypress.io/" target="_blank"><strong>Cypress</strong></a>. 
      Test runner used to validate the expected behavior of the solutions.
    </li>
  </ul>

  <h2><strong>Project Structure</strong></h2>
  <pre>
dom-manipulation/
├── cypress/               Automated test files
├── images/                Image assets
├── .editorconfig          Editor configuration
├── .eslintrc.json         JavaScript lint rules
├── .gitignore             Git ignore rules
├── .stylelintrc.json      CSS lint rules
├── README.md              Exercise documentation
├── cypress.json           Cypress configuration
├── index.html             Base HTML provided by Trybe
├── package-lock.json      Locked dependencies tree
├── package.json           Dependencies and npm scripts
├── reporter.json          Test reports
└── style.css              Main styles
  </pre>

  <h2><strong>Learning Objectives</strong></h2>
  <ul>
    <li align="justify">Practice DOM element selection using <code>id</code>, <code>className</code> and <code>tagName</code>.</li>
    <li align="justify">Modify text and styles of HTML elements using JavaScript only.</li>
    <li align="justify">Improve understanding of the DOM tree structure and navigation.</li>
    <li align="justify">Organize code into small, reusable and readable functions.</li>
    <li align="justify">Get used to technical challenge formats similar to real world hiring processes.</li>
  </ul>

  <h2><strong>How to Run</strong></h2>
  <ol>
    <li>Clone this repository or download the project files.</li>
    <li>Open <code>index.html</code> in your browser.</li>
    <li>Inspect the page and browser console to see the DOM changes applied by JavaScript.</li>
  </ol>

  <h2><strong>Project Status</strong></h2>
  <p align="justify">
    <strong>Completed</strong> as part of Trybe's Web Development course, in the JavaScript fundamentals and DOM manipulation module.
  </p>

  <h2><strong>Contact</strong></h2>
  <p>
    <strong>Willian Gonçalves</strong> |
    <a href="https://www.linkedin.com/in/williandpg/" target="_blank"><strong>LinkedIn</strong></a> |
    <a href="https://github.com/williandpg" target="_blank"><strong>Github</strong></a> |
    <a href="https://williandpg.github.io/" target="_blank"><strong>Portfolio</strong></a> |
    <a href="mailto:goncalves.wdp@outlook.com" target="_blank"><strong>Email</strong></a>
  </p>

  <h2><strong>Credits</strong></h2>
  <p align="justify">
    This exercise is based on the DOM manipulation challenge and template provided by <strong>Trybe</strong>,
    and is used here for study and practice purposes.
  </p>
</details>