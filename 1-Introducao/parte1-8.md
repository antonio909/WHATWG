# Sintaxe HTML vs XML

*Esta seção é informativa.*

Esta especificação define uma linguagem abstrata para descrever documentos e
aplicações, e algumas APIs para interagir com representação em memória de
recursos que utilizam esta linguagem.

A representação em memória é conhecida como **"DOM HTML"**, ou simplesmente **"DOM"**.

Existem várias sintaxes concretas que podem ser usadas para transmitir
recursos que utilizam esta linguagem abstrata, duas das quais são definidas
nesta especificação.

A primeira sintaxe concreta desse tipo é a **sintaxe HTML**. Este é o formato sugerido para a
maioria dos desenvolvedores. Ele é compatível com a maioria dos navegadores legados. Se um
documento for transmitido com o tipo MIME `text/html`, ele será processado como um
documento HTML pelos navegadores. Esta especificação define a sintaxe HTML mais recente,
conhecida simplesmente como 'HTML'.

A segunda sintaxe concreta é o XML. Quando um documento é transmitido com um tipo MIME
XML, como `application/xhtml+xml`, ele é tratado como um documento XML pelos
navegadores da web, para ser analisado por um processador XML. Os desenvolvedores são lembrados
de que o processamento para XML e HTML difere; em particular, mesmo erros de sintaxe
menores impedirão que um documento rotulado como XML seja renderizado totalmente, ao
passo que seriam ignorados na sintaxe HTML.

**Nota**
  A sintaxe XML para o HTML era anteriormente referida como "XHTML", mas esta especificação
  não utiliza esse termo (entre outras razões, porque tal termo não é utilizado para as sintaxes
  HTML de MathML e SVG).

O DOM, a sintaxe HTML e a sintaxe XML não podem todos representar o mesmo conteúdo. Por
exemplo, **namespaces** não podem ser representados utilizando a sintaxe HTML, mas são
suportados no DOM e na sintaxe XML.
Da mesma forma, documentos que utilizam o recurso `noscript` podem ser representados
utilizando a sintaxe HTML, mas não podem ser representados com o DOM ou na sintaxe XML.
Comentários que contêm a sequência "`<--`" só podem ser representados no DOM, e não nas
sintaxe HTML e XML.
