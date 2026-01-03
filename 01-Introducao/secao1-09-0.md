<h1>1.9 Estrutura desta especificação</h1>

<i>Esta seção é informativa.</i>

<p>Esta especificação está dividida nas seguintes seções principais:</p>

<dl>
  <dt>Introdução</dt>
  <dd>
    Materiais informativos que fornecem um contexto para o padrão HTML.
  </dd>
  <dt>Infraestrutura comum</dt>
  <dd>
    As classes de conformidade, algoritmos, definições e os fundamentos comuns do restante da especificação.
  </dd>
  <dt>Semântica, estrutura e APIs de documentos HTML</dt>
  <dd align="justify">
    Os documentos são construídos a partir de elementos.
    Esse elementos formam uma árvore utilizando o DOM.
    Esta seção define as características deste DOM, além de introduzir as funcionalidades comuns a todos os elementos e os conceitos utilizados na definição dos elementos.
  </dd>
  <dt>Os elementos do HTML</dt>
  <dd align="justify">
    Cada elemento possui um significado predefinido, que é explicado nesta seção.
    Também são fornecidas regras para autores sobre como usar o elemento, juntamente com os requisitos do agente do usuário sobre como manipular cada um deles.
    Isso inclui recursos de grande destaque do HTML, como reprodução de vídeo e legendas, controles e envio de formulários, além de uma API de gráficos 2D conhecida como HTML canvas.
  </dd>
  <dt>Microdados</dt>
  <dd align="justify">
    Esta especificação introduz um mecanismo para adicionar anotações legíveis por máquina a documentos, permitindo que ferramentas extraiam árvores de pares nome-valor do documento.
    Esta seção descreve esse mecanismo e alguns algoritmos que podem ser usados para converter documentos HTML em outros formatos.
    Esta seção também define alguns vocabulários de Microdados de exemplo para informações de contato, eventos de calendário e licenciamento de obras.
  </dd>
  <dt>Interação do usuário</dt>
  <dd align="justify">
    Documentos HTML podem fornecer uma série de mecanismos para os usuários interagirem e modificarem o conteúdo, os quais são descritos nesta seção, tais como o funcionamento do foco e o recurso de arrastar e soltar.
  </dd>
  <dt>Carregamento de páginas web</dt>
  <dd align="justify">
    Documentos HTML não existem no vácuo — esta seção define muitos dos recursos que afetam ambientes que lidam com múltiplas páginas, como navegadores da web.
  </dd>
  <dt>APIs de aplicações web</dt>
  <dd>
    Esta seção introduz recursos básicos para a criação de scripts de aplicativos em HTML.
  </dd>
  <dt>Web Workers</dt>
  <dd>
    Esta seção define uma API para threads de segundo plano em JavaScript.
  </dd>
  <dt>Worklets</dt>
  <dd align="justify">
    Esta seção define a infraestrutura para APIs que precisam executar JavaScript separadamente do ambiente principal de execução de JavaScript.
  </dd>
  <dt>As APIs de comunicação</dt>
  <dd align="justify">
    Esta seção descreve alguns mecanismos que aplicações escritas em HTML podem usar para se comunicar com outras aplicações de diferentes domínios executadas no mesmo cliente.
    Ela também introduz um mecanismo de fluxo de eventos via <i>server-push</i> conhecido como <i>Server Sent Events</i> ou <i>EventSource</i>, e um protocolo de <i>socket</i> bidirecional <i>full-duplex</i> para scripts conhecido como <i>Web Sockets</i>.
  </dd>
  <dt>Armazenamento Web</dt>
  <dd>
    Esta seção define um mecanismo de armazenamento no lado do cliente baseado em pares nome-valor.
  </dd>
  <dt>A sintaxe HTML</dt><dt>A sintaxe XML</dt>
  <dd align="justify">
    Todos esses recursos seriam inúteis se não pudessem ser representados em uma forma serializada e enviados a outras pessoas; por isso, estas seções definem as sintaxes do HTML e do XML, juntamente com as regras de como analisar o conteúdo utilizando essas sintaxes.
  </dd>
  <dt>Renderização</dt>
  <dd>
    Esta seção define as regras de renderização padrão para navegadores web.
  </dd>
</dl>

<p>Existem também alguns apêndices, listando recursos obsoletos e considerações da IANA, e vários índices.</p>
