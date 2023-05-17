# Competição kaggle - ML Olympiad for Students - TopVistos EUA

## Passo-a-passo sugerido pelos instrutores:

- 1. Métrica F1 Score = a métrica utilizada será o F1- Score. Vai depender de definir o ponto de corte, primeiramente deve otimizar o ROC AOC, pq assim vc otimiza sua performance em vários pontos de corte. Então se você otimiza essa métrica, automaticamente você otimizará o F1 Score.
  - O F1 Score é uma métrica comumente usada para avaliar a precisão de um modelo de classificação binária, considerando tanto a precisão quanto a taxa de verdadeiros positivos. O instrutor sugere otimizar a área sob a curva ROC (ROC AUC) para obter um bom desempenho em vários pontos de corte. Ao otimizar a ROC AUC, espera-se que o F1 Score também seja otimizado.

- 2. Ache o ponto de corte ideal (não necessariamente será 50%)
  - Encontrar o ponto de corte ideal: O ponto de corte é usado para definir o limite acima do qual uma instância é classificada como positiva. O instrutor menciona que o ponto de corte ideal pode não ser necessariamente 50%. Você pode ajustar o ponto de corte para otimizar o desempenho do seu modelo com base nas métricas escolhidas.

- 3. Balancear os dados = Sklearn.class_weight=True
Ele vai balancear a loss function do modelo automaticamente
  - Balanceamento dos dados: O instrutor sugere usar a opção class_weight=True do Scikit-learn para equilibrar automaticamente a função de perda do modelo. Isso é útil quando há um desequilíbrio significativo entre as classes de destino. Essa técnica permite que o modelo atribua mais importância às classes minoritárias durante o treinamento.

- 4. Algumas escalas das features terão que ser mudadas para balanceamento.
  - Escalas das features: Em alguns casos, pode ser necessário ajustar as escalas das features para melhorar o desempenho do modelo. Dependendo do algoritmo escolhido, é importante normalizar ou padronizar as features para que elas tenham uma distribuição adequada. Isso ajuda a evitar que recursos com valores maiores dominem a contribuição do modelo.

- 5. Tente criar alguma nova feature, ou remover alguma, sempre testando na validação pra ver se melhorou ou piorou (a validação local será diferente da privada, então não confie profundamente no score local), faça uma validação local de 70%, 30% dos dados de treino (validação cruzada aleatória de 3 a 5 folds localmente), em todos os testes veja se melhora ou piora localmente e no kaggle.
  - Engenharia de features: Experimentar a criação ou remoção de features é uma estratégia comum para melhorar o desempenho do modelo. Você pode criar novas features combinando ou transformando as existentes, ou remover features que não sejam relevantes para a tarefa de classificação. É importante validar localmente essas alterações usando uma divisão de dados de treinamento e validação.
  - Validação local: O instrutor sugere realizar uma validação local utilizando uma divisão de 70% dos dados para treinamento e 30% para validação. Isso pode ser feito usando validação cruzada aleatória com 3 a 5 folds. É importante avaliar o desempenho do modelo em termos de métricas relevantes, como F1 Score, em cada fold e verificar se há melhoria consistente.

- 6. Você terá 5 scores locais e mais o score do kaggle, faça uma média (5+1)/6 e veja se melhorou. No mínimo deve melhorar 3 scores locais para valer a pena.
  - Média dos scores: Para avaliar o desempenho geral do modelo, o instrutor sugere calcular a média dos scores locais e do score do Kaggle. Por exemplo, se você tiver 5 scores locais e 1 score do Kaggle, você pode calcular a média (5+1)/6. Essa média deve mostrar uma melhoria em relação aos scores locais anteriores para justificar a eficácia das alterações feitas.

- 7. Salve as previsões de cada modelo e deixando anotado as previsões, para depois ver qual é a melhor média. Ensemble, combinação de modelos.
  - Salvar as previsões: É recomendável salvar as previsões de cada modelo ao longo do processo. Dessa forma, você poderá comparar e combinar diferentes modelos posteriormente para encontrar a combinação mais eficaz. Essa etapa é conhecida como ensemble ou combinação de modelos.

  - Ao salvar as previsões de cada modelo, você pode comparar seus desempenhos individualmente e determinar quais modelos contribuem mais para melhorar o resultado geral. Você pode experimentar diferentes métodos de combinação, como votação majoritária, média das probabilidades ou até mesmo treinar um modelo adicional usando as previsões dos modelos anteriores como features.

  - Ao realizar essa combinação, é importante ter em mente que a diversidade dos modelos é fundamental. Modelos diferentes tendem a capturar informações distintas e, portanto, sua combinação pode fornecer uma visão mais abrangente dos dados.

  - Lembre-se de avaliar o desempenho do ensemble tanto localmente quanto no Kaggle para garantir que as melhorias observadas sejam consistentes em ambos os conjuntos de dados. A validação local fornece uma estimativa do desempenho do modelo em dados não vistos, enquanto o resultado no Kaggle indica como o modelo geraliza para novos dados da competição.

Em resumo, o passo-a-passo sugerido pelos instrutores envolve otimizar a métrica F1 Score, encontrar o ponto de corte ideal, balancear os dados, ajustar as escalas das features, realizar engenharia de features, validar localmente, calcular a média dos scores locais e do Kaggle e, por fim, salvar as previsões para combinar os modelos de forma eficaz. 
