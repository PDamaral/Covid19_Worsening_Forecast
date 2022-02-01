# Covid19 Worsening Forecast
Prediction of worsening health status in hospitalized infected people who may take the intensive care unit - Supervised classification (PT-BR)
## Objetivo
Iremos analisar o dataset fornecido pela equipe do Hospital Sírio Libanês, com dados anonimizados. O modelo segue as regras:
•	A feature ‘ICU’ denomina se o paciente foi transferido para a UTI.
•	Todos os dados de quando o paciente foi a UTI não devem ser usados, devido a não precisão da tomada dos mesmos, podendo comprometer a fidelidade do modelo.
•	Os dados foram agrupados em janelas de tempo na feature ‘Window’, onde são 5 janelas de tempo medidas em horas.
A estratégia para o modelo será utilizar apenas a primeira janela de tempo para realizar a predição, pois o quanto antes for tomada a decisão melhor pode ser o atendimento e a preparação da equipe medica.

## Conclusão
Obtivemos um resultado muito similar entre os datasets no modelo de regressão logística, com grau de precisão não muito alto (RECALL de 75%), porem acredito que este sistema deva ser um auxiliar a expertise do profissional de saúde, onde este conhece mais do que e possível passar a um dataset, portanto apresento a mudança da abordagem de apresentação do resultado do modelo, em vez de determinar se o paciente ira para a UTI, sera apresentada uma tabela com a chance do quadro do paciente se agravar, conforme tabela abaixo(utilizando as métricas do modelo de regressão logística com o dataset de features selecionada pelo boruta).

