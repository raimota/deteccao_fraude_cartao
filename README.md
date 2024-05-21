# Detecção de Fraudes em Transações de Cartão

## Descrição do Projeto

<p>Este projeto visa desenvolver e comparar modelos de machine learning para detectar fraudes em transações de cartão de crédito. Utilizamos técnicas de balanceamento de dados como SMOTE, ADASYN e Random Under-Sampling (RUS) para lidar com o desbalanceamento das classes e melhorar a performance dos modelos. Nosso objetivo principal é maximizar a detecção de fraudes (revocação) enquanto minimizamos falsos positivos.</p>

## Modelos Utilizados
Foram implementados e comparados os seguintes modelos de classificação:

<ul>
<li>Regressão Logística</li>
<li>Árvore de Decisão</li>
</ul>

## Técnicas de Balanceamento
As técnicas de balanceamento aplicadas foram:

<ul>
<li>Random Under-Sampling (RUS)</li>
<li>SMOTE</li>
<li>ADASYN</li>
</ul>

# Conclusão
Considerando que o objetivo principal é detectar fraudes de cartão, o modelo mais eficaz para o contexto é aquele que apresenta a melhor capacidade de identificar transações fraudulentas e ao mesmo tempo minimiza os falsos positivos, para que não gere estresse e vergonha para clientes cujas transações deveriam ser classificadas como normais.

Na avaliação dos três modelos - Regressão Logística com SMOTE, Regressão Logística com ADASYN e Regressão Logística com RUS - foi constatado que todos possuem taxas de revocação semelhantes no que se refere à eficácia na identificação de fraudes. Contudo, o modelo de Regressão Logística com ADASYN se sobressai por ter menos falsos positivos quando comparado aos demais modelos.

No cenário do modelo de Regressão Logística utilizando ADASYN, foram contabilizados 1804 casos de falsos positivos. Já nos demais modelos (Regressão Logística com SMOTE e Regressão Logística com RUS), foram registrados 1702 e 2735 falsos positivos, respectivamente. Isso indica que o modelo de Regressão Logística com ADASYN teve um desempenho superior ao identificar transações fraudulentas de forma precisa, sem incorrer em um alto índice de classificação equivocada de transações legítimas como fraudulentas.

Além do mais, o modelo de Regressão Logística utilizando ADASYN também demonstrou um AUC ligeiramente superior, indicando uma melhor habilidade geral do modelo em diferenciar entre transações legítimas e fraudulentas.

Portanto, com base nestas análises, o modelo de Regressão Logística com ADASYN é considerado o mais indicado para a detecção de fraudes em cartões.
