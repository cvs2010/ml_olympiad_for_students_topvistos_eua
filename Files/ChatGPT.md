# O Prompt Mestre:
Você é um especialista em Criação de Prompt.
Seu objetivo é me ajudar a criar o melhor prompt
possível para o que preciso
O prompt que você fornecer deve ser escrito a partir
da minha perspectiva (usuário), fazendo a
solicitação ao ChatGPT.
Considere em sua criação que esse prompt será
inserido em uma interface para GPT3, GPT4 ou
ChatGPT. Esse será o processo:
1. Você irá gerar as seguintes seções:
Prompt:
<Forneça o melhor prompt possível de acordo com
minha solicitação)
Crítica:
(Forneça um parágrafo conciso sobre como
melhorar o prompt. Seja muito crítico em sua
resposta. Esta seção destina-se a forçar a crítica
construtiva, mesmo quando o prompt é aceitável.
Quaisquer suposições e/ou problemas devem ser
incluídos)
Perguntas:
(faça quaisquer perguntas relacionadas a quais
informações adicionais são necessárias de mim
para melhorar o prompt (máximo de 3). Se o prompt
precisar de mais esclarecimentos ou detalhes em
determinadas áreas, faça perguntas para obter mais
informações para incluir no prompt)
2. Eu fornecerei minhas respostas à sua pergunta,
que você incorporará em sua próxima resposta
usando o mesmo formato. Continuaremos esse
processo iterativo comigo, te fornecendo
informações adicionais, e você atualizará o prompt
até que o prompt seja aperfeiçoado
Lembre-se, o prompt que estamos criando deve ser
escrito a partir da minha perspectiva (o usuário)
fazendo uma solicitação a você, ChatGPT (uma
interface GPT3/GPT4)
Um exemplo de prompt que você poderia criar seria
começar com "Você agirá como um físico phD para
me ajudar a entender física quântica".
Pense cuidadosamente e use sua imaginação para
criar um prompt incrível.
Sua primeira resposta deve ser apenas uma
saudação e perguntar sobre o que o prompt deve
ser.

# Prompt:
Olá! Estou aqui para te ajudar com suas dúvidas e solicitações. Por favor, me forneça informações sobre o que você precisa.
Quais são suas principais perguntas ou tópicos de interesse? Com base nisso, poderei fornecer informações relevantes e
orientações para aprofundar nossas discussões.

Crítica:
O prompt inicial fornecido é muito aberto e não oferece detalhes específicos sobre a solicitação ou o assunto em questão.
Para melhorar o prompt, é necessário fornecer informações mais específicas sobre o que você está buscando. Dessa forma, poderei
oferecer uma resposta mais direcionada e útil.

Perguntas:

Por favor, compartilhe comigo qual é o tópico ou área específica em que você precisa de ajuda ou informações.
Isso me ajudará a entender melhor sua solicitação.
Você tem alguma pergunta específica em mente ou há algo em particular que gostaria de aprender sobre o assunto?
Existe algum conceito específico que você está tendo dificuldades em entender? Se sim, por favor, forneça mais
detalhes para que eu possa focar na explicação desse conceito.
Aguardo suas respostas para que eu possa atualizar o prompt e fornecer uma orientação mais precisa e personalizada para você.

# ----
1. Competição kaggle - ML Olympiad for Students - TopVistos EUA -
https://www.kaggle.com/competitions/ml-olympiad-for-students-topvistos-eua/data?select=train.csv

2. 
- Objetivo da competição:

No ano fiscal de 2016, o OFLC processou 775.979 pedidos de empregadores para 1.699.957 posições de certificações de trabalho temporárias e permanentes. Isso representou um aumento de nove por cento no número total de pedidos processados em relação ao ano anterior. O processo de revisar cada caso está se tornando uma tarefa tediosa à medida que o número de candidatos aumenta a cada ano.

O aumento do número de candidatos a cada ano demanda uma solução baseada em Aprendizado de Máquina que possa ajudar na pré-seleção dos candidatos com maiores chances de aprovação de VISTO. O OFLC contratou sua empresa, TopVistos, para soluções baseadas em dados. Como Cientista de Dados, você deve analisar os dados fornecidos e, com a ajuda de um modelo de classificação:

Facilitar o processo de aprovação de vistos.

Recomendar um perfil adequado para os candidatos para os quais o visto deve ser certificado ou negado, com base nos fatores que influenciam significativamente o status do caso.

- Dataset Description
Os dados contêm diferentes atributos do empregado e do empregador. O dicionário de dados detalhado é fornecido abaixo.

Temos alguns arquivos disponibilizados para o treino dos modelos. Note que para seu modelo ser corretamente avaliado, você precisa enviar os seus dados no formato do arquivo sample_submission.csv.

Arquivos
train.csv - dataset de treino
test.csv - dataset de testes
sample_submission.csv - um exemplo de como o arquivo enviado deve ser composto

Dicionário dos Dados
id_do_caso: ID de cada solicitação de visto

continente: Informação do continente do empregado

educação_do_empregado: Informação sobre a educação do empregado

tem_experiência_de_trabalho: O empregado possui alguma experiência de trabalho? S = Sim; N = Não

requer_treinamento_de_trabalho: O empregado requer algum treinamento de trabalho? S = Sim; N = Não

num_de_empregados: Número de funcionários na empresa do empregador

ano_de_estabelecimento: Ano em que a empresa do empregador foi estabelecida

região_de_emprego: Informação da região de emprego pretendida pelo trabalhador estrangeiro nos EUA.

salário_prevalecente: Salário médio pago a trabalhadores em ocupações semelhantes na área de emprego pretendida. O objetivo do salário prevalecente é garantir que o trabalhador estrangeiro não seja subremunerado em comparação com outros trabalhadores que oferecem o mesmo serviço ou serviço similar na mesma área de emprego.

unidade_de_salário: Unidade do salário prevalecente. Os valores incluem Por Hora, Por Semana, Por Mês e Por Ano.

posição_em_tempo_integral: A posição de trabalho é em tempo integral? S = Posição em Tempo Integral; N = Posição em Meio Período

status_do_caso: Indicador se o visto foi certificado ou negado

3. Qual o passo-a-passo você faria utilizando o Google Colab, observando as dicas dos instrutores:

Passo-a-passo sugerido pelos instrutores:
1 - Métrica F1 Score = a métrica utilizada será o F1- Score. Vai depender de definir o ponto de corte, primeiramente deve otimizar o ROC AOC, pq assim vc otimiza sua performance em vários pontos de corte. Então se você otimiza essa métrica, automaticamente você otimizará o F1 Score.

O F1 Score é uma métrica comumente usada para avaliar a precisão de um modelo de classificação binária, considerando tanto a precisão quanto a taxa de verdadeiros positivos. O instrutor sugere otimizar a área sob a curva ROC (ROC AUC) para obter um bom desempenho em vários pontos de corte. Ao otimizar a ROC AUC, espera-se que o F1 Score também seja otimizado.
2 - Ache o ponto de corte ideal (não necessariamente será 50%)

Encontrar o ponto de corte ideal: O ponto de corte é usado para definir o limite acima do qual uma instância é classificada como positiva. O instrutor menciona que o ponto de corte ideal pode não ser necessariamente 50%. Você pode ajustar o ponto de corte para otimizar o desempenho do seu modelo com base nas métricas escolhidas.
3 - Balancear os dados = Sklearn.class_weight=True Ele vai balancear a loss function do modelo automaticamente

Balanceamento dos dados: O instrutor sugere usar a opção class_weight=True do Scikit-learn para equilibrar automaticamente a função de perda do modelo. Isso é útil quando há um desequilíbrio significativo entre as classes de destino. Essa técnica permite que o modelo atribua mais importância às classes minoritárias durante o treinamento.
4 - Algumas escalas das features terão que ser mudadas para balanceamento.

Escalas das features: Em alguns casos, pode ser necessário ajustar as escalas das features para melhorar o desempenho do modelo. Dependendo do algoritmo escolhido, é importante normalizar ou padronizar as features para que elas tenham uma distribuição adequada. Isso ajuda a evitar que recursos com valores maiores dominem a contribuição do modelo.
5 - Tente criar alguma nova feature, ou remover alguma, sempre testando na validação pra ver se melhorou ou piorou (a validação local será diferente da privada, então não confie profundamente no score local), faça uma validação local de 70%, 30% dos dados de treino (validação cruzada aleatória de 3 a 5 folds localmente), em todos os testes veja se melhora ou piora localmente e no kaggle.

Engenharia de features: Experimentar a criação ou remoção de features é uma estratégia comum para melhorar o desempenho do modelo. Você pode criar novas features combinando ou transformando as existentes, ou remover features que não sejam relevantes para a tarefa de classificação. É importante validar localmente essas alterações usando uma divisão de dados de treinamento e validação.
Validação local: O instrutor sugere realizar uma validação local utilizando uma divisão de 70% dos dados para treinamento e 30% para validação. Isso pode ser feito usando validação cruzada aleatória com 3 a 5 folds. É importante avaliar o desempenho do modelo em termos de métricas relevantes, como F1 Score, em cada fold e verificar se há melhoria consistente.
6 - Você terá 5 scores locais e mais o score do kaggle, faça uma média (5+1)/6 e veja se melhorou. No mínimo deve melhorar 3 scores locais para valer a pena.

Média dos scores: Para avaliar o desempenho geral do modelo, o instrutor sugere calcular a média dos scores locais e do score do Kaggle. Por exemplo, se você tiver 5 scores locais e 1 score do Kaggle, você pode calcular a média (5+1)/6. Essa média deve mostrar uma melhoria em relação aos scores locais anteriores para justificar a eficácia das alterações feitas.
7 - Salve as previsões de cada modelo e deixando anotado as previsões, para depois ver qual é a melhor média. Ensemble, combinação de modelos.

Salvar as previsões: É recomendável salvar as previsões de cada modelo ao longo do processo. Dessa forma, você poderá comparar e combinar diferentes modelos posteriormente para encontrar a combinação mais eficaz. Essa etapa é conhecida como ensemble ou combinação de modelos.

Ao salvar as previsões de cada modelo, você pode comparar seus desempenhos individualmente e determinar quais modelos contribuem mais para melhorar o resultado geral. Você pode experimentar diferentes métodos de combinação, como votação majoritária, média das probabilidades ou até mesmo treinar um modelo adicional usando as previsões dos modelos anteriores como features.

Ao realizar essa combinação, é importante ter em mente que a diversidade dos modelos é fundamental. Modelos diferentes tendem a capturar informações distintas e, portanto, sua combinação pode fornecer uma visão mais abrangente dos dados.

Lembre-se de avaliar o desempenho do ensemble tanto localmente quanto no Kaggle para garantir que as melhorias observadas sejam consistentes em ambos os conjuntos de dados. A validação local fornece uma estimativa do desempenho do modelo em dados não vistos, enquanto o resultado no Kaggle indica como o modelo geraliza para novos dados da competição.

Em resumo, o passo-a-passo sugerido pelos instrutores envolve otimizar a métrica F1 Score, encontrar o ponto de corte ideal, balancear os dados, ajustar as escalas das features, realizar engenharia de features, validar localmente, calcular a média dos scores locais e do Kaggle e, por fim, salvar as previsões para combinar os modelos de forma eficaz.
