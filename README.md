# fiap-pos-tech-ai-scientist-fase-1-desafio
Desafio Tech da fase 1 da pós-tech em AI Scientist pela FIAP.

Você deverá atender os seguintes requisitos nesse desafio:
1. Entendimento do negócio: nessa primeira etapa, queremos exercitar o seu pensamento analítico, não código. Nos traga a resposta para as seguintes perguntas de negócio:
  ● Qual problema de negócio está sendo resolvido?
  ● Por que o NPS é importante para um e-commerce?
  ● Quais áreas poderiam se beneficiar desses insights? Exemplos: logística, atendimento, pricing, produto etc.

Além do entendimento do negócio, inclua uma reflexão (não precisa de dados externos obrigatórios):
Como o NPS impacta:
  ● Recompra;
  ● Boca a boca;
  ● Market share em e-commerce.

Quais indicadores de mercado poderiam complementar essa análise? Exemplos: benchmarks de NPS, SLA logístico, concorrência.

2. Definição da Target: qual é o alvo desse problema de negócio? Nessa segunda etapa queremos uma avaliação de entendimento conceitual, não técnico.
  ● Qual variável representa a satisfação do cliente?
  ● Por que ela foi escolhida?
  ● Em que momento da jornada essa informação é coletada?
  ● Existe algum risco de usar essa variável de forma inadequada?

4. Análise Exploratória dos Dados (EDA): realize uma análise exploratória com foco em negócio, não só estatística. Responda:
  ● Quais fatores parecem mais críticos para a satisfação?
  ● O que mais gera detratores?
  ● Existe algum “ponto de ruptura” na experiência do cliente?
  ● Que tipo de cliente tende a ter NPS mais alto ou mais baixo?

Imagine que você está explicando isso para um(a) gerente de operações que não entende estatística.

4. Como forma de preparação para as próximas fases do curso, este desafio propõe uma reflexão prática sobre como a Ciência de Dados pode ser utilizada para antecipar a satisfação do cliente.

A partir da dor de negócio apresentada neste case, reflita sobre como um modelo preditivo poderia apoiar a empresa a prever o NPS antes da aplicação da pesquisa. Considere diferentes abordagens possíveis, como:
  ● Um modelo de regressão, para estimar a nota de NPS em uma escala contínua;
  ● Um modelo de classificação, para categorizar clientes, por exemplo, em satisfeitos e insatisfeitos.
  
Descreva qual estratégia você adotaria para resolver esse problema utilizando dados e Inteligência Artificial, justificando suas escolhas do ponto de vista técnico e de negócio.
Caso opte por implementar a solução, apresente uma proposta de modelo aplicada em Python, explicando de forma clara:
  ● A definição da variável alvo;
  ● A seleção e preparação das variáveis de entrada;
  ● A lógica de separação dos dados (quando aplicável);
  ● A escolha do modelo;
  ● A forma de avaliação dos resultados;
  ● E como essa solução poderia ser utilizada na prática pela empresa.

Este desafio (4) é opcional e tem como objetivo ampliar a maturidade analítica e técnica, sem impacto negativo para quem optar por não realizá-lo.

Base de dados
Acesse o arquivo CSV com dados históricos de pedidos, entregas e interações com o atendimento ao cliente.

Arquivo: Base de dados NPS
Exemplos de informações disponíveis:
  ● Dados do pedido (valor, quantidade de itens, forma de pagamento);
  ● Dados logísticos (tempo de entrega, atraso, tentativas);
  ● Dados de atendimento (contatos, tempo de resolução);
  ● Indicadores internos de negócio.

Dicionário de Dados
  ● customer_id: Identificador único do cliente.
  ● order_id: Identificador único do pedido.
  ● customer_age: Idade do cliente.
  ● customer_region: Região geográfica do cliente.
  ● customer_tenure_months: Tempo de relacionamento do cliente com a empresa (em meses).
  ● order_value: Valor total do pedido.
  ● items_quantity: Quantidade de itens no pedido.
  ● discount_value: Valor de desconto aplicado ao pedido.
  ● payment_installments: Número de parcelas do pagamento.
  ● delivery_time_days: Tempo total de entrega (em dias).
  ● delivery_delay_days: Quantidade de dias de atraso na entrega.
  ● freight_value: Valor do frete.
  ● delivery_attempts: Número de tentativas de entrega.
  ● customer_service_contacts: Número de contatos do cliente com o atendimento.
  ● resolution_time_days: Tempo para resolução de problemas (em dias).
  ● complaints_count: Número de reclamações registradas pelo cliente.
  ● repeat_purchase_30d: Indica se houve recompra em até 30 dias após o pedido (0 = não, 1 = sim).
● csat_internal_score: Score interno de satisfação do cliente.
● nps_score: Nota de satisfação do cliente (NPS), variando de 0 a 10, coletada após a experiência de compra.
