# Extensibilidade

*Esta seção é informativa.*

O HTML possui uma ampla variedade de mecanismos de extensibilidade que
podem ser usados para adicionar semântica de maneira segura:

* Os desenvolvedores podem usar o atributo `class` para estender elementos, criando efetivamente
  seus próprios elementos, ao mesmo tempo em que utilizam o elemento HTML 'real' mais
  aplicável, para que navegadores e outras ferramentas que não conheçam a extensão ainda
  possam suportá-la razoavelmente bem. Essa é a abordagem usada por 'microformats', por
  exemplo.

* Os desenvolvedores podem incluir dados para processamento por scripts *inline* do lado do cliente ou
  scripts do lado do servidor em todo o site usando os atributos `data-*=""`. É garantido que
  esses atributos nunca serão alterados pelos navegadores, permitindo que scripts incluam
  dados em elementos HTML para que, posteriormente, esses mesmos scripts possam localizá-
  los e processá-los.

* Os desenvolvedores podem utilizar o mecanismo `<meta name="" content="">` para incluir metadados
  em toda a página.

* Os desenvolvedores podem usar o mecanismo **`rel=""`** para anotar links com significados específicos,
  registrando extensões para o conjunto predefinido de tipos de link. Isso também é utilizado
  por **microformats**.

* Os desenvolvedores podem incorporar dados brutos usando o mecanismo `<script
  type="">` com um tipo personalizado, para posterior manipulação por scripts
  internos ou do lado do servidor.

* Desenvolvedores podem estender APIs utilizando o mecanismo de prototipagem
  (prototyping) do JavaScript. Isso é amplamente utilizado por bibliotecas de
  scripts, por exemplo.

* Os desenvolvedores podem usar o recurso de **microdados** (os atributos `itemscope=""` e
  `itemprop=""`) para incorporar pares nome-valor de dados aninhados para serem
  compartilhados com outras aplicações e sites.

* Os desenvolvedores podem definir, compartilhar e usar elementos personalizados (custom elements)
  para estender o vocabulário do HTML. Os requisitos para nomes válidos de elementos
  personalizados garantem a compatibilidade futura (uma vez que nenhum elemento será
  adicionado ao HTML, SVG ou MathML com nomes locais contendo hífen no futuro).
