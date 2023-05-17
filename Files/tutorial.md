# Competição kaggle - ML Olympiad for Students - TopVistos EUA

## Passo-a-passo sugerido pelos instrutores:

- Métrica F1 Score = a métrica utilizada será o F1- Score. Vai depender de definir o ponto de corte, primeiramente deve otimizar o ROC AOC, pq assim vc otimiza sua performance em vários pontos de corte. Então se você otimiza essa métrica, automaticamente você otimizará o F1 Score.

- Ache o ponto de corte ideal (não necessariamente será 50%)

- Balancear os dados = Sklearn.class_weight=True
Ele vai balancear a loss function do modelo automaticamente

- Algumas escalas das features terão que ser mudadas para balanceamento.

- Tente criar alguma nova feature, ou remover alguma, sempre testando na validação pra ver se melhorou ou piorou (a validação local será diferente da privada, então não confie profundamente no score local), faça uma validação local de 70%, 30% dos dados de treino (validação cruzada aleatória de 3 a 5 folds localmente), em todos os testes veja se melhora ou piora localmente e no kaggle.

- Você terá 5 scores locais e mais o score do kaggle, faça uma média (5+1)/6 e veja se melhorou. No mínimo deve melhorar 3 scores locais para valer a pena.

- Salve as previsões de cada modelo e deixando anotado as previsões, para depois ver qual é a melhor média. Assemble, combinação de modelos.
