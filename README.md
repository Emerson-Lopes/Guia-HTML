# **Guia de Referências do HTML**
HTML é uma linguagem de marcação utilizada na construção de páginas na Web. Documentos HTML podem ser interpretados por navegadores.

É essencial para todo desenvolvedor web ser proficiente em HTML. E mesmo que HTML não seta tão difícil de aprender é comum esquecer tudo que a linguagem de marcação tem para oferecer. Uma boa prática é sempre ter um guia de referência disponível para solucionar qualquer problema.
## **Sintaxe - Estrutura - Padrões**
### **Sumário do Guia**
Vamos ver como podemos quebrar o código em componentes diferentes:

`<html>...</html>`
Esta tag especifica que a página foi escrita em HTML. Ela aparece na primeira linha da página. É utilizada prinicipalmente para mostrar que a página usa HTML5 - a versão mais recente da linguagem. Também conhecido como elemento root, esta tag pode ser considerada como uma tag pai para qualquer outra tag na página.

`<head>...</head>`
Esta tag é utilizada para especificar dados meta sobre a página. Ela inclui o nome da página, suas dependências (JS e scrips CSS), uso de fonte, etc.

`<title>...</title>`
Como o nome sugere, esta tag contém o título/nome da página. Você pode ver isso na barra de navegação do navegador para qualquer página aberta. Mecanismos de busca utilizam esta tag para extrair o assunto da página, o que é bastante conveniente para ranqueamento.

`<body>...</body>`
Tudo que p usuário vê é escrito dentro desta tag, que contém todos os conteúdos da página.

#### **Exemplo:**
```
<html>
    <head>
        <title>Seu primeiro HTML</title>
    </head>
    <body>
        <p>Aqui é onde as coisas acontecem, o corpo de seu HTML</p>
    </body>
</html>
```

### **Informações do Guia**

`<base/>`
Utilizada para especificar a URL base do seu site, esta tag faz a linkagem com links internos mais limpas.

`<meta/>`
Esta é a tag do meta da página. Pode ser utíl para mencionar o autor da página, pelavras-chave, datas de publicação original. etc.

`<links/>`
Utilizada para linkar com links externos à página. Tipicamente usada para inclusão de stylesheets.

`<style>...</style>`
A tag `style` pode ser utilizada com uma alternativa à uma stylesheet externa, ou para complementá-la. Inclui as informações de aparência da página.

`<script>...</script>`
Utilizada para adicionar códigos snippet tipicamente em JavaScript, para tornar a página dinâmica. Também pode ser usada para linkar à um script externo.

#### **Exemplo:**
```
<html>
    <head>
        <meta charser="utf-8">
        <base href="https://meuprimeirosite.com" target="_blank">
        <title>Meu Website</title>
        <link rel="stylesheet" href="/css/master.css">
        <script type="text/javascript">
            var dummy = 0;
        </script>
    </head>
    <body>

    </body>
</html>
```

### **Estrutura do Guia**

`<h1..h6>...</h1..h6>`
Seis variações de escrita de cabeçalho. O `<h1>` possui o maior tamanho de fonte, enquanto o `<h6>` o menor.

`<div>...</div>`
O conteúdo de uma página é geralmente dividido em blocos, especificados pela tag `div`.

`<span>...</span>`
Esta tag insere elementos de linha, como uma imagem, ícone e emoticon, sem estragar aformatação/estilo da página.

`<p>...</p>`
Texto sem formatação é colocado dentro desta tag.

`<br/>`
Quebra de linha para uma página, Utilizado quando você quer escrever em uma nova linha.

`<hr/>`
Parecida com a tag acima. Mas em adição à pular linha, esta tag também desenha uma barra horizontal indicando o fim da seção.

#### **Exemplo:**
```
<div>
    <h1>5 Maiores Filmes </h1>
    <p>Esses são considerados os 5 maiores filmes<span>reel-icon</span>de todos os tempos </p>
    <hr/>
    <h2>1. The Godfather</h2>
    <p>O clássico de 1972 possui no elencon Marlon Brando e Al Pacino.< /p>
</div>
```

### **Formatação de Texto**

`<strong>...</strong>`
Deixaa o texto em negrito. Usado para enfatizar o conteúdo.

`<b>...</b>`
Alternativa à tag acima, também deixa o texto em negrito.

`<em>...</em>`
Outra tag para enfatizar, mas esta mostra o texto em itálico.

`<i>...</i>`
Também mostra o texto em itálico, mas não enfatiza como a tag acima.

`<cite>...</cite>`
Tag para citar o autor de uma frase.

`<del>...</del>`
Texto préformatado "monoespaço" apresentado com espaço em branco dentro do elemento intacto.

`<ins>...</inst>`
Denota um texto que foi inserido na página.

`<blockquote>...</blockquote>`
Citações são geralmente colocadas com esta tag. Ela é utilizada em conjunto com a tag `<cite>`.

`<q>...</q>`
Parecida com a tag acima, mas citações menores.

`<abbr>...</abbr>`
Denota abreviações, juntamente com a forma completa.

`<address>...</address>`
Tag para especificar as informações de contato do autor.

`<dfn>...</dfn>`
Tag dedicada para definições.

`<code>...</code>`
Utilizada para mostrar códigos snippet dentro de um parágrafo.

`<sub>...</sub>`
Tag para escrita de um subscript (um texto de fonte menor logo abaixo da fonte principal).

`<sup>...</sup>`
Similar com a tag anterior, mas para superscript(texto acima).

`<small>...</small>`
Reduz o tamanho do texto. No HTML5 geralmente se refere à informações redundantes ou inválidas.

#### **Exemplo:**
```
<p><strong>Texto em negrito </strong> Regular text<em>texto em itálico </em> texto normal</p>

<blockquote>Tudo deveria se tornar o mais simples possível, mas não simplificado.<cite>- Albert Einstein</cite></blockquote>

<pre>Texto pré-formatado</pre>

<p><code>algum código </code></p>
```

### **Links**

`<a href="">...</a>`
Tag âncora. Principalmente utilizada para inclusão de hyperlinks.

`<a href="mailto:">...</a>`
Tag dedicada para envio de emails.

`<a href="tel:####-####">...</a>`
Tag âncora para menção de números de contato. Como os números são clicáveis, é particulamente útil para usuários de celular.

`<a name="name">...</a>`
Esta tag pode ser utilizada para navegação rápida para outra parte da página.

`<a href="#name">...</a>`
Uma variação da tag acima, sendo utilizada somente para navegação de uma seção.

### **Imagens**

`<img>`
Tag para mostrar imagens em uma página.

`src="url"`
A URL ou caminho onde a imagem está localizada no seu drive ou na web.

`alt="text"`
O texto escrito aqui é exibido quando o usuário passa o mouse em cima da imagem. Pode ser utilizada para dar detalhes adicionais sobre a imagem e boa prática para acessibilidade.

`height="value"`
Especifica a altura da imagem em pixels ou porcentagem.

`width="value"`
Especifica a largura da imagem em pixels ou porcetagem.

`align="value"`
O alinhamento relativo da imagem. Pode mudar com a alteração de outros elementos na página.

`border="value"`
Especifica a grossura da borda da imagem. Se não definido fica com o padrão 0.

`<map>...</map>`
Denota uma imagem interativa (clicável).

`<map name="value">...</map>`
Nome do mapa assiado entre a imagem e o mapa.

`<area>`
Especifica a área da imagem do mapa.

`shape="value"`
Formato da área.

`coords="value"`
Coordinadas da informação vital do formato. Exemplo: vértices para triângulos, centro/radianos para círculos.

#### **Exemplo:**
```
<img src="planets.gif" width="145" height="126 alt="Planets" usemap="#planetmap">
<map name="planetmap">
    <area shape="rect" coords="0,0,60,100" href="sun.htm" alt="Sun">
    <area shape="circle" coords="90,58,3"href="mercur.htm" alt="Mercury">
    <area shape="circle" coords="124,58,8"href="venus.htm" alt="Venus">
</map>
```

### **Listas**

`<ol>...</ol>`
Tag para lista ordenadas ou numeradas de itens.

`<ul>...</ul>`
Contrária à tag acima, esta é para itens desordenados.

`<li>...</li>`
Item individual como parte da lista.

`<dl>...</dl>`
Tag para listas de itens com definições.

`<dt>...</dt>`
A difinição de um único termo em linha com conteúdo.

`<dd>...</dd>`
A descrição do termo definido.

#### **Exemplo:**

```
<ol>
    <li>Segunda</li>
    <li>Terça</li>
    <li>Quarta</li>
</ol>
<ul>
    <li>França</li>
    <li>Alemanha</li>
    <li>Itália</li>
</ul>
<dl>
    <dt>Toyota</dt>
    <dd>Marca de carro japonesa</dd>
    <dt>Armani</dt>
    <dd>Marca de roupa italiana</dd>
</dl>
```
### **Formulários**

`<form>...</form>`
A tag pai de um formulário HTML.

`action="url"`
A URL listada aqui é onde os dados do formulários serão enviados assim que preenchidos pelo usuário.

`method="..."`
Especifica qual método HTTP(POST ou GET) é utilizado para envio de formulário.

`enctype="..."`
Apenas para métodos POST, a tag dita o esquema de codificação para ser usado quando o formulário é enviado.

`autocomplete`
Determina se o formulário possui preenchimento automático habilitado.

`novalidate`
Dtermina se o formulário deve ser validado antes do envio.

`accept-charsets`
Determina a codificação dos caracteres quando o formulário é enviado.

`target`
Após o envio, a resposta do formulário é mostrada para onde a tag se refere, geralmente possui os seguintes valores: `values: _blank, _self, _parent, _top`.

`<fieldset>...</fieldset>`
Identifica o grupo de todos os campos no formulário.

`<label>...</label>`
É utilizado para marcar um campo no formulário.

`<legend>...</legend>`
Opera como legenda para o elemento `<fieldset>`.

`<input/>`
Esta tag é utilizada para receber informações (input) do usuário. O tipo de informação é determinado por um número de atributos.

### **Atributos Tipo `input`**










### Tags
`<!DOCTYPE html>` Tem a função de indicar ao navegador qual tipo de página ele irá renderizar<br>
`<head>` Cabeça (contém informações sobre a sua página)<br>
`<body>` Corpo (é o que será exibido no navegador)<br>
`<h1>` Títulos que temos 6 níveis de subtítulos<br>
`<p>` Parágrafo<br>
`<a href="">` Âncora (para links) com o atributo `href` cria-se um hiperligação nas páginas web<br>
`<ol>` Listas Ordenadas<br>
`<ul>` Listas não Ordenadas<br>
`<dl>` Lista de Definições<br>
`<table>` Tabela<br>
`<tbody>` Corpo da Tabela<br>
`<tr>` Linha da Tabela<br>
`<td>` Coluna da Tabela<br>
`<thead>` Cabeçalho da Tabela<br>
`<th>` Define o titulo de cada coluna<br>
`<tfoot>` Rodapé da Tabela<br>
`<img src="">` Imagem<br>
`<center>` Centralizar HTML<br>
`<meta>` O elemento define qualquer informação de metadados que não podem ser definidos por outro elementos HTML<br>
`<title>` Título da página web<br>
`<header>` Cabeçalho do Layout<br>
`<section>` Sessão do Layout<br>
`<nav>` Navegação do Layout<br>
`<article>` Artigo do Layout<br>
`<aside>` Representa uma seção de uma página que consiste de conteúdo que é tangencialmente relacionado ao conteúdo do seu entorno<br>
`<footer>` Rodapé do Layout<br>