# ModelandoDBmecanica
Modelando o banco de dados de uma mecânica - DIO Heineken 

# Requisitos do Sistema de controle e gerenciamento de execução de ordens de serviço em uma oficina mecânica

- Clientes levam veículos à oficina mecânica para serem consertados ou para passarem por revisões periódicas: um veículo deve ser atribuído a apenas um cliente, ao passo que um cliente pode levar vários veículos. O tipo de serviço (conserto ou revisão) está definido na ordem de serviço "gerada" pelo veículo.
- Cada veículo é designado a uma equipe de mecânicos que identifica os serviços a serem executados e preenche uma OS com data de entrega: vários mecânicos são atribuídos a várias tarefas. Essa atribuição é composta por um mecânico, um veículo e um tipo de tarefa (avaliação do veículo ou execução de serviço).
- A partir da OS, calcula-se o valor de cada serviço, consultando-se uma tabela de referência de mão-de-obra: valores dos serviços estão definidos na própria entidade "Serviço". Compõe parte do valor da OS.
- O valor de cada peça também irá compor a OS: valores das peças estão definidos na própria entidade "Peça". Compõe parte do valor da OS.
- O cliente autoriza a execução dos serviços: autorização representada pelo relacionamento "gera" entre veículo e ordem de serviço.
- Os mecânicos possuem código, nome, endereço e especialidade: atributos da entidade "Mecânico".
- Cada OS possui: n°, data de emissão, um valor, status e uma data para conclusão dos trabalhos: atributos da entidade "Ordem de serviço".
