<h1>1.9.1 Como ler esta especificação</h1>

<p align="justify">
  Esta especificação deve ser lida como todas as outras.
  Primeiro, deve ser lida do início ao fim, várias vezes.
  Depois, deve ser lida de trás para frente pelo menos uma vez.
  Em seguida, deve ser lida escolhendo seções aleátorias da lista de conteúdos e seguindo todas as referências cruzadas.
</p>

<p align="justify">
  Como descrito na seção de requisitos de conformidade abaixo, esta especificação descreve critérios de conformidade para uma variedade de classes de conformidade.
  Em particular, existem requisitos de conformidade que se aplicam aos <b>produtores</b> (por exemplo, autores e documentos que eles criam) e requisitos que se aplicam aos <b>consumidores</b> (por exemplo, navegadores web).
  Eles podem ser distinguidos pelo que estão exigindo: um requisito para um produtor estabelece o que é <b>permitido</b>, enquanto um requisito para um consumidor estabelece como o software deve <b>agir</b>.
</p>

<dl>
  <dt>Exemplo</dt>
  <dd align="justify">
    Por exemplo, "o valor do atributo <code>foo</code> deve ser um número inteiro válido" é um requisito para <b>produtores</b>, pois define os valores permitidos; em contraste, o requisito "o valor do atributo <code>foo</code> deve ser analisado utilizando as regras para análise de inteiros" é um requisito para <b>consumidores</b>, pois descreve como processar o conteúdo.
  </dd>
</dl>

<p>
  <strong>As exigências feitas aos produtores não têm qualquer impacto sobre os consumidores.</strong>
</p>

<dl>
  <dt>Exemplo</dt>
  <d align="justify">
    Continuando o exemplo acima, um requisito que estabelece que o valor de um atributo específico está restrito a ser um número inteiro válido, enfaticamente, não implica nada sobre os requisitos impostos aos consumidores.
    Pode ser que os consumidores sejam, na verdade, obrigados a tratar o atributo como uma string opaca, permanecendo totalmente indiferentes ao fato de o valor estar ou não em conformidade com os requisitos.
    Pode ser também (como no exemplo anterior) que os consumidores sejam obrigados a analisar o valor utilizando regras específicas que definem como valores inválidos (neste caso, não numéricos) devem ser processados.
  </d>
</dl>
