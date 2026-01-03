<h1>1.7.1 Serialização da execução de scripts</h1>

<i>Esta seção é informativa.</i>

<p align="justify">
  Para evitar expor os autores da web às complexidades do <b>multithreading</b> (múltiplas threads), as APIs de HTML e DOM são projetadas de forma que nenhum script possa detectar a execução simultânea de outros scripts.
  Mesmo com o uso de <b>workers</b>, a intenção é que o comportamento das implementações possa ser pensado como uma serialização completa da execução de todos os scripts em todos os escopos globais.
</p>

<p align="justify">
  A exceção a este princípio geral de design é a classe <strong>SharedArrayBuffer</strong> do JavaScript.
  Ao utilizar objetos SharedArrayBuffer, pode-se, de fato, observar que scripts em outros agentes estão sendo executados simultaneamente.
  Além disso, devido ao modelo de memória do JavaScript, existem situações que não são apenas irrepresentáveis via execução de script serializada, mas tambem irrepresentáveis via execução de instruções serializadas entre esses scripts.
</p>
