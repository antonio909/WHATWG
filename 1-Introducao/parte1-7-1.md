# Serialização da execução de scripts

*Esta seção é informativa.*

Para evitar expor os desenvolvedores web às complexidades do multithreading (múltiplas
threads), as APIs de HTML e DOM são projetadas de tal forma que nenhum script
possa detectar a execução simultânea de outros scripts. Mesmo com o uso de
workers, a intenção é que o comportamento das implementações possa ser
interpretado como uma serialização completa da execução de todos os scripts em
todos os contextos globais.

A exceção a este princípio geral de design é a classe *SharedArrayBuffer* do JavaScript. Ao
utilizar objetos *SharedArrayBuffer*, é possível observar, de fato, que scripts em outros
agentes estão sendo executados simultaneamente. Além disso, devido ao modelo de memória
do JavaScript, existem situações que não apenas são irrepresentáveis via execução de script
serializada, mas também irrepresentáveis via execução de instrução serializada entre esses
scripts.
