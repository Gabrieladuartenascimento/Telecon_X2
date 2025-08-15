# Telecon_X2

## Relatório Detalhado: Análise dos Fatores de Evasão e Estratégias de Retenção

Com base na análise dos dados de evasão de clientes e no desempenho dos modelos de Regressão Logística e Random Forest, identificamos os seguintes fatores que mais influenciam a evasão:

### Principais Fatores que Influenciam a Evasão

Analisando a importância das features em ambos os modelos:

*   **Tempo de Contrato (tenure):** Este é um dos fatores mais consistentes e importantes. Clientes com menor tempo de contrato demonstram uma maior propensão a evadir.
*   **Faturamento Mensal e Faturamento Total:** Ambas as métricas de faturamento são relevantes. A Regressão Logística deu alta importância ao Faturamento Mensal, enquanto o Random Forest destacou o Faturamento Total. Isso sugere que o valor que o cliente representa e seu padrão de gastos estão relacionados à sua decisão de permanecer ou sair.
*   **Serviço de Internet (Fiber Optic):** A análise de Regressão Logística indicou que ter o serviço de internet via fibra óptica está associado a uma maior probabilidade de evasão. Isso pode apontar para questões específicas de satisfação com este tipo de serviço.
*   **Método de Pagamento (Electronic Check):** Clientes que utilizam o pagamento eletrônico mostraram maior tendência à evasão, um fator com alta importância no modelo Random Forest.
*   **Tipo de Contrato (Two Year Contract):** Ter um contrato de dois anos é um forte indicativo de menor evasão, um fator importante em ambos os modelos, o que faz sentido dado o compromisso de longo prazo.

### Desempenho dos Modelos

*   O modelo **Random Forest** teve um desempenho geral superior no conjunto de teste balanceado, com uma acurácia de aproximadamente **84.2%**.
*   O modelo de **Regressão Logística** obteve uma acurácia de aproximadamente **80.4%**.

O Random Forest demonstrou ser um pouco mais eficaz em prever a evasão neste dataset específico.

### Estratégias de Retenção Propostas

Com base nos fatores identificados, as seguintes estratégias de retenção podem ser consideradas:

*   **Programas de Onboarding e Engajamento para Novos Clientes:** Desenvolver iniciativas direcionadas a clientes nos primeiros meses de contrato (`tenure` baixo) para aumentar o engajamento e a lealdade.
*   **Investigação e Melhoria do Serviço de Fibra Óptica:** Realizar pesquisas de satisfação e investigar possíveis problemas técnicos ou de atendimento relacionados ao serviço de fibra óptica para reduzir a insatisfação dos clientes.
*   **Incentivos para Contratos de Longo Prazo:** Promover ativamente os contratos de um ou dois anos com benefícios exclusivos para aumentar a retenção a longo prazo.
*   **Análise e Otimização do Processo de Pagamento Eletrônico:** Investigar as razões por trás da maior evasão entre usuários de pagamento eletrônico. Simplificar o processo, oferecer suporte em caso de problemas e garantir transparência nas cobranças podem ajudar.
*   **Segmentação e Ofertas Baseadas no Valor do Cliente:** Utilizar as métricas de faturamento para segmentar clientes e oferecer programas de fidelidade ou serviços personalizados que atendam às necessidades de diferentes perfis de gastos.

Este relatório resume as principais descobertas e sugere direções para ações de retenção.
