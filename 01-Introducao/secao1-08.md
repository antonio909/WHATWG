<h1>1.8 Sintaxe HTML vs. XML</h1>

<i>Esta seção é informativa.</i>

<p align="justify">
  Esta especificação define uma linguagem abstrata para descrever documentos e aplicações, além de algumas APIs para interação com representações em memória de recursos que utilizam esta linguagem.
</p>

<p align="justify">
  A representação em memória é conhecida como "DOM HTML", ou simplesmte "o DOM".
</p>

<p align="justify">
  Existem várias sintaxes concretas que podem ser usadas para transmitir recursos que utilizam esta linguagem abstrata, duas das quais são definidas nesta especificação.
</p>

<p align="justify">
  A primeira dessas sintaxes concretas é a <b>sintaxe HTML</b>.
  Este é o formato sugerido para a maioria dos autores.
  Ele é compatível com a maioria dos navegadores legados.
  Se um documento for transmitido com o tipo MIME <code>text/html</code>, ele será processado pelos navegadores como um documento HTML.
  Esta especificação define a sintaxe HTML mais recente, conhecida simplesmente como "HTML".
</p>

<p align="justify">
  A segunda sintaxe concreta é o <b>XML</b>.
  Quando um documento é transmitido com um tipo MIME XML, como <code>application/xhtml+xml</code>, ele é tratado como um documento XML pelos navegadores da web, para ser analisado por um processador XML.
  Os autores são lembrados de que o processamento para XML e HTML difere; em particular, <strong>mesmo pequenos erros de sintaxe impedirão que um documento rotulado como XML seja totalmente renderizado</strong>, ao passo que seriam ignorados na sintaxe HTML.
</p>

<p align="justify">
  <strong>Nota:</strong> A sintaxe XML para o HTML era anteriormente referida como "XHTML", mas esta especificação não utiliza esse termo (entre outros motivos, porque tal termo não é utilizado para as sintaxes HTML de MathML e SVG).
</p>

<p align="justify">
  O DOM, a sintaxe HTML e a sintaxe XML não conseguem representar todos os mesmo conteúdo.
  Por exemplo, os <b>namespaces</b> não podem ser representados usando a sintaxe HTML, mas são suportados no DOM e na sintaxe XML.
  Da mesma forma, documentos que utilizam o recurso <b>noscript</b> podem ser representados usando a sintaxe HTML, mas não podem ser representados com o DOM ou na sintaxe XML.
  Comentários que contêm a sequência de caracteres "<code>--&gt;</code>" só podem ser representados no DOM, e não nas sintaxes HTML e XML.
</p>
