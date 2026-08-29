# fiap-pos-tech-ai-scientist-fase-1-desafio
Desafio Tech da fase 1 da pós-tech em AI Scientist pela FIAP.

  O presente estudo tem por objetivo analisar os fatores que influenciam o Net Promoter Score (NPS), buscando compreender o comportamento dos clientes e identificar as tendências ao longo de sua jornada de compra no e-commerce.
  Mais do que realizar uma análise puramente descritiva, busca-se formular as perguntas certas para identificar relações e possíveis fatores associados ao NPS. A análise conjunta dos dados disponíveis pode revelar oportunidades de melhoria em aspectos como logística, atendimento, prazo de entrega, experiência de compra e satisfação, transformando os dados em insights relevantes para o negócio.
  Um NPS elevado tende a estar associado a uma maior propensão à recompra, uma vez que clientes satisfeitos tendem a manter uma relação de lealdade com a empresa. Também pode favorecer o boca a boca, por meio de recomendações e avaliações positivas, contribuindo para a conquista de novos consumidores. No contexto do e-commerce, esses dois efeitos, de maior retenção e maior aquisição por recomendação, podem contribuir, no médio e longo prazos, para o crescimento das vendas e do market share. Essa relação, entretanto, deve ser investigada nos dados, pois NPS elevado não implica, por si só, causalidade sobre recompra ou participação de mercado.
  Os insights produzidos podem ser utilizados por praticamente toda a cadeia do negócio, especialmente a de experiência do cliente. A logística pode identificar o impacto de prazos e atrasos, o atendimento pode entender o impacto da quantidade de contatos e tempo de resolução das demandas, o comercial pode mapear os fatores que aumentam a retenção e o potencial de vendas, como descontos e condições de pagamento.
  A análise poderá ser mais completa se incluir aspectos de comparação com indicadores externos, permitindo contextualizar os resultados obtidos:
* Benchmark de NPS: comparação com a média do setor e com concorrentes;
* Concorrência: market share, crescimento, preços, frete e prazos de entrega dos principais players;
* Fatores macroeconômicos, que explicam as tendências de mercado e consumo.

  A variável que representa a satisfação do cliente é o NPS, que consiste na nota atribuída pelo cliente à sua propensão a recomendar a empresa. O cliente atribui a nota após o encerramento da jornada de compra, e a partir dela, é classificado em promotor (9 a 10), neutro (7 a 8) ou detrator (abaixo de 6).
  Entre os dados obtidos, o NPS foi escolhido por ser um indicador amplamente utilizado para avaliar a percepção, lealdade e propensão à recomendação do cliente em relação ao e-commerce. Para este estudo, ele permite investigar quais características da jornada de compra estão associadas a uma experiência positiva ou negativa.
  O principal risco é tratar o NPS como uma medida absoluta de satisfação ou como uma variável que, isoladamente, explica o comportamento futuro do cliente. Um NPS elevado não garante, por exemplo, que haverá recompra, assim como um NPS baixo não significa necessariamente que o cliente deixará de comprar.
  Também é importante considerar que o NPS pode ser influenciado pelo momento e pelo contexto em que a pesquisa é realizada, além de possíveis vieses de resposta. Por isso, a análise deve considerar outras variáveis.
Dessa forma, o objetivo não é apenas prever ou explicar uma nota de NPS, mas identificar os fatores da jornada que estão associados à percepção do cliente e que podem representar oportunidades concretas de melhoria para o negócio.






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
