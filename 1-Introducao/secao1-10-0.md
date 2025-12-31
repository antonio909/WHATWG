<h1 align="center">Uma rápida introdução ao HTML</h1>

<p align="center"><i>Esta seção é informativa.</i></p>

<p align="justify">Um documento HTML básico se parece com isto:</p>

```
<!DOCTYPE html>
<html lang="en">
 <head>
  <title>Sample page</title>
 </head>
 <body>
  <h1>Sample page</h1>
  <p>This is a <a href="demo.html">simple</a> sample.</p>
  <!-- this is a comment -->
 </body>
</html>
```

<p align="justify">
  Os documentos HTML consistem em uma árvore de elementos e texto.
  Cada elemento é indicado no código-fonte por uma tag de abertura, como <code>&lt;body&gt;</code>, e uma tag de fechamento, como <code>&lt;/body&gt;</code>.
  (Certas tags de abertura e fechamento podem, em alguns casos, ser omitidas e são implícitas por outras tags).
</p>

<p align="justify">
  As tags devem ser aninhadas de forma que os elementos fiquem completamente uns dentro dos outros, sem se sobrepor.
</p>

```
<p>This is <em>very <strong>wrong</em>!</strong></p>

<p>This <em>is <strong>correct</strong>.</em></p>
```

<p align="justify">
  Esta especificação define um conjunto de elementos que podem ser usados no HTML, juntamente com regras sobre as maneiras pelas quais os elementos podem ser aninhados.
</p>

<p align="justify">
  Os elementos podem ter <b>atributos</b>, que controlam como os elementos funcionam.
  No exemplo, há um link (hyperlink), formado usando o elemento <code>&lt;a&gt;</code> e seu atributo <code>href</code>:
</p>

```
<a href="demo.html">simple</a>
```

<p align="justify">
  Os atributos são colocados dentro da tag de abertura e consistem em um nome e um valor, separados por um caractere '<code>=</code>'.
  O valor do atributo pode permanecer sem aspas se não contiver espaços em branco ASCII ou qualquer um dos caracteres <code>" ' ` = &lt;</code> ou <code>&gt;</code>.
  Caso contrário, ele deve ser colocado entre aspas simples ou duplas.
  O valor, junto com o caractere '<code>=</code>', pode ser omitido inteiramente se o valor for uma string vazia.
</p>

```
<!-- empty attributes -->
<input name=address disabled>
<input name=address disabled="">

<!-- attributes with a value -->
<input name=address maxlength=200>
<input name=address maxlength='200'>
<input name=address maxlength="200">
```

<p align="justify">
  Os agentes de usuário HTML (ex: navegadores web) então analisam essa marcação, transformando-a em uma árvore <b>DOM (Document Object Model)</b>.
  Uma árvore DOM é uma representação do documento na memória.
</p>

<p align="justify">
  As árvores DOM contém vários tipos de nós, em particular um nó <code>DocumentType</code>, nós de <b>Elemento</b>, nós de <b>Texto</b>, nós de <b>Comentário</b> e, em alguns casos, nós de <code>ProcessingInstruction</code>.
</p>

<p align="justify">
  O trecho de marcação no topo desta seção seria transformado na seguinte árvore DOM:
</p>

```
DOCTYPE: html
html lang="en"
  head
    #text: ⏎␣␣
    title
      #text: Sample page
    #text: ⏎␣
  #text: ⏎␣
  body
    #text: ⏎␣␣
    h1
      #text: Sample page
    #text: ⏎␣␣
    p
      #text: This is a
      a href="demo.html"
        #text: simple
      #text: sample.
    #text: ⏎␣␣
    #comment: this is a comment
    #text: ⏎␣⏎
```

<p align="justify">
  O elemento de documento desta árvore é o elemento <code>html</code>, que é o elemento sempre encontrado nessa posição em documentos HTML.
  Ele contém dois elementos, <code>head</code> e <code>body</code>, bem como um nó de <code>Text</code> entre eles.
</p>

<p align="justify">
  Existem muito mais nós de texto (<i>Text nodes</i>) na árvore DOM do que se esperaria inicialmente, porque o código-fonte contém uma série de espaços (representados aqui por "_") e quebras de linha ('⏎') que acabam se tornando nós de texto no DOM.
  No entanto, por razões históricas, nem todos os espaços e quebras de linha da marcação original aparecem no DOM.
  Em particular, todo o espaço em branco antes da tag de abertura <code>head</code> acaba sendo descartado silenciosamente, e todo o espaço em branco após a tag de fechamento <code>body</code> acaba sendo colocado ao final do corpo (<i>body</i>).
</p>

<p align="justify">
  O elemento <code>head</code> contém um elemento <code>title</code>, que por sua vez contém um nó de texto (<i>Text node</i>) com o texto '<code>Sample page</code>'.
  Da mesma forma, o elemento <code>body</code> contém um elemento <code>h1</code>, um elemento <code>p</code> e um comentário.
</p>
