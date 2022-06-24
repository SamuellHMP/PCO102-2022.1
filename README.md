# PCO102-2022.1
Atividades de Inteligência Artificial do POSCOMP Unifei

# Introdução
Este trabalho propõe como problema de pesquisa a aplicação de ferramentas de Inteligência Artificial (IA) na análise do perfil do operador de caminhão-fora-de-estrada de mineração. Pretendo utilizar o dataset escolhido para aplicar diferentes algoritmos de IA para classificar o comportamento do condutor do veículo em ambientes virtuais de simulação computacional. Futuramente, pretendo expandir essa aplicação para conseguir avaliar o desempenho dos condutores de caminhões-fora-de-estrada durante treinamendos usando simuladores.

Busca-se desenvolver um modelo otimizado de operação desses caminhões considerando a necessidade de aumentar a produtividade, diminuir o tempo ocioso, reduzir custos de operação e manutenção e aprimorar a segurança. Esta proposta trabalha com uma área de pesquisa ainda pouco explorada, de alta complexidade, devido aos parâmetros envolvidos e de grande valor para as empresas de mineração, fornecendo informações úteis de gestão para recrutar, acompanhar e avaliar os recursos humanos envolvidos na operação dessa importante parte da frota mineira. 

Os resultados dessa pesquisa também podem auxiliar trabalhos da área da computação, notadamente na simulação da operação e na automação desses caminhões, bem como na virtualização de um ambiente real de mineração. Esta proposta está alinhada com o projeto de pesquisa do qual eu participo e sou bolsista e estou envolvido no desenvolvimento de um sistema supervisório para um sistema de simulação de caminhões-fora-de-estrada CAT-793F em ambientes de mineração.

A partir das referências [3-9], são revisados os dois métodos de Inteligência Artificial adotados para abordar o problema, Redes Neurais Artificiais e Correlação Cruzada, bem como são referenciados trabalhos recentes sobre cada um dos métodos. 

# Justificativa
De acordo com o website da mineradora Vale [1], seus maiores consumos energéticos são em eletricidade e em diesel. Este último é utilizado principalmente como combustível nos caminhões fora de estrada e nas locomotivas, participando de 24% do total do consumo energético. Além do combustível, toda máquina apresenta gastos com manutenção e substituição das peças que a compõem. A mineradora também está preocupada com a sustentabilidade de seus negócios, buscando estratégias para reduzir a emissão de gases do efeito estufa [1]. Geralmente, as empresas mineradoras possuem programas de eficiência energética que abrangem toda a matriz energética e esta pesquisa pode auxiliar estas empresas a serem mais eficientes na utilização de energia para atingirem as desafiadoras metas de sustentabilidade e, ao mesmo tempo, contribuir para o aumento de competitividade mediante a redução de custos operacionais. 

Outros elementos que corroboram esta proposta estão relacionados às tendências tecnológicas da área da mineração. O cenário futuro da mineração aponta para a utilização de veículos autônomos e virtualização de ambientes reais de mineração [2]. As máquinas não precisarão de operadores humanos para funcionar, porém, para atingir isso, um caminho possível se inicia em se entender como o operador humano se comporta e qual é o modelo ótimo de operação dessas máquinas para depois construir softwares capazes de substituir os seres humanos nesta tarefa. 

# Revisão Bibliográfica

Há trabalhos sobre a aplicação de RNAs na engenharia de minas [3], engenharia bioquímica [4], medicina [5] e engenharia mecânica [6]. 

As RNAs também são conhecidas como redes neurais, redes neurais simuladas ou processamento paralelo distribuído e podem ser entendidas como modelos matemáticos que imitam algumas das características conhecidas dos sistemas nervosos naturais do ser humano e esboçam as analogias do aprendizado natural adaptativo. O principal componente de um paradigma de RNA particular pode ser a estrutura incomum do sistema de processamento de dados. Há um grupo de modelos que imita algumas das características conhecidas dos sistemas nervosos naturais e se baseia nas analogias do aprendizado natural adaptativo. O principal componente de um paradigma de RNA particular pode ser a estrutura incomum do sistema de processamento de dados. Um modelo neuronal típico é, portanto, composto de conectores ponderados, um somador e uma função de ativação. 

A parte principal de uma estrutura de rede neural é um 'nó'. Os nós biológicos geralmente somam os sinais recebidos de várias fontes de maneiras diferentes e, em seguida, realizam uma ação não linear nos resultados para criar as saídas. RNAs normalmente têm uma camada de entrada, uma ou mais camadas ocultas e uma camada de saída. Cada entrada é multiplicada por seu peso conectado e, no estado mais simples, essas quantidades e vieses são combinados; eles então passam pelas funções de ativação para criar a saída. 

Em resumo, existem alguns fundamentos para a aplicação de RNAs: são modelos tolerantes a falhas e simples que não requerem informações para identificar os parâmetros relacionados; não precisam da descrição matemática dos fenômenos envolvidos no processo; e são utilizadas em várias aplicações de computador para resolver problemas complexos.

Correlação cruzada são usadas para calcular e representar graficamente as correlações entre duas séries temporais em diferentes períodos de tempo. A representação gráfica das correlações cruzadas pode ajudar a determinar se uma série de dados conduz outra série, e até que ponto. Por exemplo, um engenheiro ambiental usa correlação cruzada para medir o sedimento em suspensão na água em dois locais de um rio durante mais de quinze dias. O engenheiro espera uma correlação entre os dois locais. Como um desses locais fica mais longe rio abaixo, o engenheiro espera que o padrão de correlação seja consistente com o tempo necessário para que a água se mova entre os dois locais.

Aplicações de classificação por correlação cruzada podem ser encontradas nos trabalhos [7], em que se conseguiu uma alta acurárica, notadamente com o algoritmo KNN (K Nearest Neigbor) de 99%, e no trabalho [8], que corrobora o anterior, simplificando o modelo e obtendo também uma alta acurária.

O KNN é um algoritmo não pramétrico, onde a estrutura do modelo será determinada pelo dataset utilizado. Este algoritmo também é conhecido como de aprendizado lento (lazy). Os algoritmos do tipo lazy, não necessitam de dados de treinamento para se gerar o modelo, o que diminui em partes o processo inicial, mas em contrapartida gerará uma necessidade de análise posterior mais apurada. No caso de algoritmos que não necessitam de treinamento, todos os dados obtidos no dataset serão utilizados na fase de teste, resultando em um treinamento muito rápido e em um teste e validação lentos.

No algoritmo KNN possuímos uma variável chamada de K, a qual é parte do nome do modelo e também o principal parâmetro a ser selecionado. Este parâmetro direcionará a quantidade de vizinhos (neighborn em inglês). Em casos de modelos binários, aonde possuímos apenas duas classes, em geral aplica-se valores ímpares a K.

# Base de Dados
O dataset escolhido para este trabalho "Carla Driver Behaviour Dataset" foi coletado para classificar diferentes comportamentos de motoristas. A plataforma de simulação "Carla Simulator" foi usada para coletar os dados através de sensores virtuais de 6 eixos, sendo 3 eixos do acelerêmetro e 3 eixos do giroscópio.

O ambiente de coleta de dados com o simulador Carla foi aplicado ao mapa "Town03". O modelo do carro escolhido para a coleta foi o "Seat Leon". O carro foi dirigido por 7 motoristas diferentes, no mesmo caminho por 5 voltas. A coluna "class" contem os primeiros nomes dos motoristas: [ mehdi, apo, gonca, onder, berk, selin, hurcan]

O autor do dataset é Mehdi Özel, @dasmehdixtr, e está disponível no kaggle no seguinte link: https://www.kaggle.com/datasets/dasmehdixtr/carla-driver-behaviour-dataset. O autor deixa registrado no site que seu dataset é livre para propósitos acadêmicos.

# Metodologias
Foram escolhidas duas metodologias para abordar o problema: redes neurais artificiais e correlação cruzada, disponíveis em [7] e [9], respectivamente. Abaixo essas metodologias são discutidas brevemente.

1. Redes Neurais Artificiais (RNAs) são um método de Inteligência Artificial para simular o efeito de múltiplas variáveis em um parâmetro principal por uma função de aptidão. Elas fornecem soluções desejáveis para problemas complexos, pois podem interpretar as relações compostas entre os vários parâmetros envolvidos em um problema. Uma das principais vantagens das RNAs é que elas podem simular tanto relações lineares quanto relações não lineares entre parâmetros, usando as informações fornecidas para treinar a rede. São também conhecidas como processamento paralelo distribuído e basicamente são a representação algorítmica de métodos que o cérebro humano usa para aprender. RNAs são redes de sistemas de computação compostas de uma série de elementos de processamento simples e altamente interconectados, que processam informações buscando respostas dinâmicas para entradas externas. Caracterizam-se por ser modelos simples e tolerantes a falhas que não requerem informações para identificar os parâmetros relacionados e não requerem a descrição matemática dos fenômenos envolvidos no processo.

2. Em processamento de sinais, relação cruzada ou correlação cruzada é uma medida de similaridade entre dois sinais em função de um atraso aplicado a um deles. Também é conhecida como produto interno deslizante. A relação cruzada é frequentemente utilizada quando se deseja procurar por um sinal de curta duração que esteja inserido em um sinal mais longo. A relação cruzada é muito semelhante em natureza à convolução de duas funções. Porém, ao contrário da convolução, na relação cruzada não há espelhamento de um dos sinais. Outra importante propriedade que distingue estas duas operações é que a convolução é comutativa, o mesmo não ocorre na relação cruzada. Quando ambas as funções de entrada em uma relação cruzada são a mesma função, a relação cruzada é conhecida por autocorrelação.

# Resultados Baseados em Métricas

Baseado no código disponível em [10] foram criados gráficos de acurácia e perda nos conjuntos de treinamento e validação. Os gráficos mostram que a precisão do treinamento e a precisão da validação estão com grandes margens, e o modelo alcançou apenas cerca de 26% de precisão no conjunto de validação.

Logo após, o modelo é refeito aumentando o número de épocas de 10 para 20, e, com isso, obteve-se uma acurácia de quase 30%.

Com a visualização dos gráficos de acurácia e perda, é possível perceber que o modelo parece convergir para uma melhor acurária à medida que o número de épocas aumenta, porém, isso acontece lentamente. Em [7], o autor chegou a executar o modelo para 1100 épocas, obtendo uma acurácia de quase 55%.

Pode-se concluir que este modelo de Rede Neural Artificial não é o melhor classificador para o dataset trabalhado, e veremos a seguir modelos que alcançam uma taxa de acurária muito melhor com menos esforço computacional.

Com o modelo proposto em [9] foi possível obter uma acurácia muito melhor do que o primeiro, chegando a uma acurária de aproximadamente 84% para o método SVM e quase 100% para o KNN.

# Conclusão

O melhor modelo de classificação dentre os aplicados é o KNN com uma acurácia de quase 100%.

Como limitação, cito a falta de capacidade para aplicar a métrica das curvas ROC, que foram indicadas pelo professor, porém, acredito que devido ao dataset ser muito grande, com várias classes, essa métrica se mostrou difícil de ser aplicada. Na tentativa, ao construir o vetor de previsões, depois de 40 minutos, o algoritmo não convergiu e abortei o processo.

Como trabalhos futuros, que devem estar dentro da minha proposta de dissertação, acredito que consistirão na aplicação das técnicas e conceitos apreendidos com este trabalho no contexto que a dissertação se propõe, que acredito ser um caso mais específico do que foi trabalhado aqui.  

# Referências
Segue abaixo a lista das referências utilizadas nesta proposta, na ordem em que aparecem no texto. As duas primeiras são de websites brasileiros e as demais são de artigos científicos internacionais sobre o tema, levantados no banco de dados Scopus, da editora Elsevier. 

[1] VALE. Energia, Consumo e Eficiência energética. Disponível em: http://www.vale.com/brasil/PT/business/energy/Paginas/default.aspx Acesso em: 08/12/2021. 

[2] NOGUEIRA, Bruna. Veículos autônomos já são realidade na mineração. Disponível em: https://revistamineracao.com.br/2017/12/05/veiculos-autonomos-ja-sao-realidade-na-mineracao/ Acesso em: 08/12/2021. 

[3] Soofastaei, A., Aminossadati, S.M., Arefi, M.M. and Kizil, M.S., Development of a multi-layer perceptron artificial neural network model to determine haul trucks energy consumption. International Journal of Mining Science and Technology, (2016). 26(2): P. 285-293. 

[4] Talib, A., Abu Hasan, Y. and Abdul Rahman, N., Predicting biochemical oxygen demand as indicator of river pollution using artificial neural networks, in 18th World Imacs/Modsim Congress. 2009: Cairns, Australia: p. 195-202. 

[5] McCulloch, W. and Pitts, W., A logical calculus of the ideas immanent in nervous activity. The Bulletin of Mathematical Biophysics, 1943, 5(4): p. 115-133. 

[6] Beigmoradi, S., Hajabdollahi, H. and Ramezani, A., Multi-objective aero acoustic optimisation of rear end in a simplified car model by using hybrid robust parameter design, artificial neural networks and genetic algorithm methods. Computers and Fluids, 2014, 90: p. 123-132.

[7] Ozel, Mehdi. Driver Classification via Neural Networks. Disponível em: https://www.kaggle.com/code/dasmehdixtr/driver-classification-via-neural-networks. Acesso em: 08/06/2022.

[8] Ozel, Mehdi. High Accuracy Classification via Cross-Correlation. Disponível em: https://www.kaggle.com/code/dasmehdixtr/high-accuracy-classification-via-cross-corrleation. Acesso em 08/06/2022.

[9] Ishan, Kumar. Minor Project Model via Cross-Correlation. Disponível em: https://www.kaggle.com/code/ishankumar2001/minor-project-model-via-cross-corrleation. Acesso em 08/06/2022.

[10] TensorFlow. Classificação de imagem. Disponível em: https://www.tensorflow.org/tutorials/images/classification. Acesso em: 23/06/2022.
