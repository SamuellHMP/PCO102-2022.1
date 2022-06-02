# PCO102-2022.1
Atividades de Inteligência Artificial do POSCOMP Unifei

# Introdução
Este trabalho propõe como problema de pesquisa a aplicação de ferramentas de Inteligência Artificial (IA) na análise do perfil do operador de caminhão-fora-de-estrada de mineração. Pretendo utilizar o dataset escolhido para aplicar diferentes algoritmos de IA para classificar o comportamento do condutor do veículo em ambientes virtuais de simulação computacional. Futuramente, pretendo expandir essa aplicação para conseguir avaliar o desempenho dos condutores de caminhões-fora-de-estrada durante treinamendos usando simuladores.

Busca-se desenvolver um modelo otimizado de operação desses caminhões considerando a necessidade de aumentar a produtividade, diminuir o tempo ocioso, reduzir custos de operação e manutenção e aprimorar a segurança. Esta proposta trabalha com uma área de pesquisa ainda pouco explorada, de alta complexidade, devido aos parâmetros envolvidos e de grande valor para as empresas de mineração, fornecendo informações úteis de gestão para recrutar, acompanhar e avaliar os recursos humanos envolvidos na operação dessa importante parte da frota mineira. 

Os resultados dessa pesquisa também podem auxiliar trabalhos da área da computação, notadamente na simulação da operação e na automação desses caminhões, bem como na virtualização de um ambiente real de mineração. Esta proposta está alinhada com o projeto de pesquisa do qual eu participo e sou bolsista e estou envolvido no desenvolvimento de um sistema supervisório para um sistema de simulação de caminhões-fora-de-estrada CAT-793F em ambientes de mineração. 

# Justificativa
De acordo com o website da mineradora Vale [1], seus maiores consumos energéticos são em eletricidade e em diesel. Este último é utilizado principalmente como combustível nos caminhões fora de estrada e nas locomotivas, participando de 24% do total do consumo energético. Além do combustível, toda máquina apresenta gastos com manutenção e substituição das peças que a compõem. A mineradora também está preocupada com a sustentabilidade de seus negócios, buscando estratégias para reduzir a emissão de gases do efeito estufa [1]. Geralmente, as empresas mineradoras possuem programas de eficiência energética que abrangem toda a matriz energética e esta pesquisa pode auxiliar estas empresas a serem mais eficientes na utilização de energia para atingirem as desafiadoras metas de sustentabilidade e, ao mesmo tempo, contribuir para o aumento de competitividade mediante a redução de custos operacionais. 

Outros elementos que corroboram esta proposta estão relacionados às tendências tecnológicas da área da mineração. O cenário futuro da mineração aponta para a utilização de veículos autônomos e virtualização de ambientes reais de mineração [2]. As máquinas não precisarão de operadores humanos para funcionar, porém, para atingir isso, um caminho possível se inicia em se entender como o operador humano se comporta e qual é o modelo ótimo de operação dessas máquinas para depois construir softwares capazes de substituir os seres humanos nesta tarefa. 

# Revisão Bibliográfica
A partir das referências [3-10], os dois métodos de Inteligência Artificial mais importantes para esta proposta de pesquisa são explicados a seguir, bem como são referenciados trabalhos recentes sobre cada um dos métodos. 

Redes Neurais Artificiais (RNAs) são um método de Inteligência Artificial para simular o efeito de múltiplas variáveis ​​em um parâmetro principal por uma função de aptidão. Elas fornecem soluções desejáveis ​​para problemas complexos, pois podem interpretar as relações compostas entre os vários parâmetros envolvidos em um problema. Uma das principais vantagens das RNAs é que elas podem simular tanto relações lineares quanto relações não lineares entre parâmetros, usando as informações fornecidas para treinar a rede. São também conhecidas como processamento paralelo distribuído e basicamente são a representação algorítmica de métodos que o cérebro humano usa para aprender. 

RNAs são redes de sistemas de computação compostas de uma série de elementos de processamento simples e altamente interconectados, que processam informações buscando respostas dinâmicas para entradas externas. Caracterizam-se por ser modelos simples e tolerantes a falhas que não requerem informações para identificar os parâmetros relacionados e não requerem a descrição matemática dos fenômenos envolvidos no processo. Há trabalhos sobre a aplicação de RNAs na engenharia de minas [3], engenharia bioquímica [4], medicina [5] e engenharia mecânica [6]. 

As RNAs também são conhecidas como redes neurais, redes neurais simuladas ou processamento paralelo distribuído e podem ser entendidas como modelos matemáticos que imitam algumas das características conhecidas dos sistemas nervosos naturais do ser humano e esboçam as analogias do aprendizado natural adaptativo. O principal componente de um paradigma de RNA particular pode ser a estrutura incomum do sistema de processamento de dados. Há um grupo de modelos que imita algumas das características conhecidas dos sistemas nervosos naturais e se baseia nas analogias do aprendizado natural adaptativo. O principal componente de um paradigma de RNA particular pode ser a estrutura incomum do sistema de processamento de dados. Um modelo neuronal típico é, portanto, composto de conectores ponderados, um somador e uma função de ativação. 

A parte principal de uma estrutura de rede neural é um 'nó'. Os nós biológicos geralmente somam os sinais recebidos de várias fontes de maneiras diferentes e, em seguida, realizam uma ação não linear nos resultados para criar as saídas. RNAs normalmente têm uma camada de entrada, uma ou mais camadas ocultas e uma camada de saída. Cada entrada é multiplicada por seu peso conectado e, no estado mais simples, essas quantidades e vieses são combinados; eles então passam pelas funções de ativação para criar a saída. 

Em resumo, existem alguns fundamentos para a aplicação de RNAs: são modelos tolerantes a falhas e simples que não requerem informações para identificar os parâmetros relacionados; não precisam da descrição matemática dos fenômenos envolvidos no processo; e são utilizadas em várias aplicações de computador para resolver problemas complexos. 

O Algoritmo Genético (AG) fornece um método para resolver problemas de otimização, imitando o processo evolutivo com base na mecânica da seleção natural de Darwin. Esses algoritmos buscam métodos baseados em princípios de seleção natural e genética [7]. Os AGs podem ser categorizados como meta-heurísticas com perspectiva global e têm sido aplicados a uma ampla gama de problemas científicos, de engenharia e econômicos [8]. 

Recentemente, os AGs têm recebido considerável atenção quanto ao seu potencial como técnica de otimização para problemas complexos e têm sido aplicados com sucesso na área de engenharia industrial [9]. Eles são implementados como uma simulação de computador para encontrar as melhores soluções e codificam as variáveis ​​de decisão de um problema de pesquisa em cadeias de caracteres de comprimento finito de alfabetos de certa cardinalidade. 

As strings, que são soluções candidatas para o problema de pesquisa, são referidas como cromossomos. Os alfabetos são chamados de genes e os valores dos genes são chamados de alelos. Em contraste com as técnicas de otimização tradicionais, os AGs trabalham com a codificação de parâmetros, ao invés dos próprios parâmetros. 

Para desenvolver boas soluções e implementar a seleção natural, é essencial ter uma medida para distinguir boas soluções de soluções ruins. A medida pode ser uma função objetiva que é um modelo matemático ou uma simulação de computador, ou pode ser uma função subjetiva onde os humanos escolhem soluções melhores em vez de piores. Em essência, a medida de aptidão deve determinar a aptidão relativa de uma solução candidata, que será posteriormente usada pelo AG para orientar a evolução de boas soluções. 

Outro conceito importante de AGs é a noção de população [10]. Ao contrário dos métodos de pesquisa tradicionais, os algoritmos genéticos dependem de uma população de soluções candidatas. O tamanho da população, que geralmente é um parâmetro especificado pelo usuário, é um dos parâmetros importantes que afetam a escalabilidade e o desempenho dos algoritmos genéticos. Uma vez que o problema é codificado de forma cromossômica e uma medida de adequação para discriminar as soluções boas das ruins foi escolhida, a evolução geralmente começa a partir de uma população de indivíduos gerados aleatoriamente e acontece em gerações.  

Em cada geração, a aptidão de cada indivíduo na população é avaliada, vários indivíduos são selecionados estocasticamente da população atual (com base em sua aptidão) e modificados para formar uma nova população. A nova população é então usada na próxima iteração do algoritmo. Normalmente, o algoritmo termina quando um número máximo de gerações foi produzido ou um nível de aptidão satisfatório foi alcançado para a população. 

Algumas terminologias básicas para Algoritmos Genéticos são apresentadas a seguir: 

Função de avaliação (fitness): é a função que se deseja otimizar. Para algoritmos de otimização padrão, ela é conhecida como função objetivo; 

Indivíduos: é qualquer ponto ao qual pode-se aplicar a função de avaliação. O valor da função de aptidão para um indivíduo é sua pontuação. Um indivíduo às vezes é referido como um genoma e as entradas de vetores de um indivíduo como genes; 

Populações e gerações: uma população é um conjunto de indivíduos. A cada iteração, o algoritmo genético realiza uma série de cálculos na população atual para produzir uma nova população. Cada população sucessiva é chamada de nova geração; 

Diversidade: refere-se à distância média entre indivíduos em uma população. Uma população tem alta diversidade se a distância média for grande; 

Valor de aptidão: é o valor da função de aptidão para determinado indivíduo; 

Pais e filhos: para criar a próxima geração, o algoritmo genético seleciona certos indivíduos na população atual, chamados pais, e os usa para criar indivíduos na próxima geração, chamados filhos. Normalmente, o algoritmo tem maior probabilidade de selecionar pais com melhores valores de aptidão. 

As etapas a seguir podem ser aplicadas para usar o Algoritmo Genético em projetos industriais: 

Inicialização: a população inicial de soluções candidatas é gerada aleatoriamente no espaço de pesquisa. No entanto, o conhecimento específico do domínio ou outras informações podem ser facilmente incorporados. 

Avaliação: uma vez que a população é inicializada ou uma população descendente é criada, os valores de aptidão das soluções candidatas são avaliados. 

Seleção: a seleção aloca mais cópias dessas soluções com valores de adequação mais altos e, portanto, impõe o mecanismo de sobrevivência do mais apto às soluções candidatas. A ideia principal é escolher as melhores soluções dentre as piores, e muitos procedimentos de seleção foram propostos para realizar essa ideia, incluindo seleção de roleta, seleção universal estocástica, seleção de classificação e seleção de torneio. 

Recombinação: a recombinação combina partes de duas ou mais soluções parentais para criar soluções novas e possivelmente melhores (ou seja, descendência). Existem muitas maneiras de fazer isso, e o desempenho competente depende de um mecanismo de recombinação adequadamente projetado. A prole sob recombinação não será idêntica a nenhum pai em particular e, em vez disso, combinam características parentais de uma maneira nova. 

Mutação: enquanto a recombinação opera em dois ou mais cromossomos parentais, a mutação local, aleatoriamente, modifica uma solução. Novamente, existem muitas variações de mutações, mas geralmente envolve uma ou mais mudanças feitas nas características de um indivíduo. Em outras palavras, a mutação executa uma passagem aleatória nas proximidades de uma solução candidata. 

Substituição: a população descendente criada por seleção, recombinação e mutação substitui a população parental original. O algoritmo geralmente seleciona indivíduos com melhores valores de aptidão como pais. O AG cria três tipos de filhos para a próxima geração: 

Crianças de elite são os indivíduos da geração atual com os melhores valores de condicionamento físico. Esses indivíduos sobrevivem automaticamente até a próxima geração. 

Crianças cruzadas são criadas combinando os vetores de um par de pais. 

Os filhos da mutação são criados pela introdução de alterações aleatórias, ou mutações, a um único pai. 

Os AGs diferem da otimização convencional e do procedimento de busca em várias maneiras fundamentais, como listado a seguir: 

Trabalham com uma codificação de conjunto de soluções, não com as próprias soluções; 

Buscam uma população de soluções, não uma única solução; 

Usam informações de payoff (função de avaliação), não derivadas ou outro conhecimento auxiliar; 

Usam regras de transição probabilísticas, não regras determinísticas. 

Os AGs têm recebido atenção considerável em relação ao seu potencial como uma nova técnica de otimização. Existem quatro vantagens principais ao aplicar algoritmos genéticos para otimização de problemas: 

Não têm muitos requisitos matemáticos sobre os problemas de otimização. Devido à sua natureza evolutiva, os AGs irão buscar soluções sem se preocupar com as especificidades internas do funcionamento do problema; 

Podem lidar com qualquer tipo de função objetivo e qualquer tipo de restrição (ou seja, linear ou não linear) definidas em espaços de busca discretos, contínuos ou mistos; 

A periodicidade dos operadores de evolução torna os AGs muito eficazes na execução de pesquisas globais (em probabilidade); 

Os AGs fornecem uma grande flexibilidade para hibridizar com heurísticas dependentes de domínio para fazer uma implementação eficiente para um problema específico.

# Base de Dados
O dataset escolhido para este trabalho "Carla Driver Behaviour Dataset" foi coletado para classificar diferentes comportamentos de motoristas. A plataforma de simulação "Carla Simulator" foi usada para coletar os dados através de sensores virtuais de 6 eixos, sendo 3 eixos do acelerêmetro e 3 eixos do giroscópio.

O ambiente de coleta de dados com o simulador Carla foi aplicado ao mapa "Town03". O modelo do carro escolhido para a coleta foi o "Seat Leon". O carro foi dirigido por 7 motoristas diferentes, no mesmo caminho por 5 voltas. A coluna "class" contem os primeiros nomes dos motoristas: [ mehdi, apo, gonca, onder, berk, selin, hurcan]

O autor do dataset é Mehdi Özel, @dasmehdixtr, e está disponível no kaggle no seguinte link: https://www.kaggle.com/datasets/dasmehdixtr/carla-driver-behaviour-dataset. O autor deixa registrado no site que seu dataset é livre para propósitos acadêmicos.

# Referências
Segue abaixo a lista das referências utilizadas nesta proposta, na ordem em que aparecem no texto. As duas primeiras são de websites brasileiros e as demais são de artigos científicos internacionais sobre o tema, levantados no banco de dados Scopus, da editora Elsevier. 

[1] VALE. Energia, Consumo e Eficiência energética. Disponível em: http://www.vale.com/brasil/PT/business/energy/Paginas/default.aspx Acesso em: 08/12/2021. 

[2] NOGUEIRA, Bruna. Veículos autônomos já são realidade na mineração. Disponível em: https://revistamineracao.com.br/2017/12/05/veiculos-autonomos-ja-sao-realidade-na-mineracao/ Acesso em: 08/12/2021. 

[3] Soofastaei, A., Aminossadati, S.M., Arefi, M.M. and Kizil, M.S., Development of a multi-layer perceptron artificial neural network model to determine haul trucks energy consumption. International Journal of Mining Science and Technology, (2016). 26(2): P. 285-293. 

[4] Talib, A., Abu Hasan, Y. and Abdul Rahman, N., Predicting biochemical oxygen demand as indicator of river pollution using artificial neural networks, in 18th World Imacs/Modsim Congress. 2009: Cairns, Australia: p. 195-202. 

[5] McCulloch, W. and Pitts, W., A logical calculus of the ideas immanent in nervous activity. The Bulletin of Mathematical Biophysics, 1943, 5(4): p. 115-133. 

[6] Beigmoradi, S., Hajabdollahi, H. and Ramezani, A., Multi-objective aero acoustic optimisation of rear end in a simplified car model by using hybrid robust parameter design, artificial neural networks and genetic algorithm methods. Computers and Fluids, 2014, 90: p. 123-132. 

[7] Gen, M. and Cheng, R., Genetic algorithms and engineering optimization. Vol. 7. 2000, New York City: John Wiley and Sons: p. 185-210. 

[8] Sánchez, D., Melin, P., Castillo, O. and Valdez, F., Modular neural networks optimization with hierarchical genetic algorithms with fuzzy response integration for pattern recognition, in Advances in Computational Intelligence. 2013, Springer: p. 247-258. 

[9] Tancret, F., Combination of Computational Thermodynamics, Gaussian Processes and Genetic Algorithms for Superalloy Design, in TMS 2013 142nd Annual Meeting and Exhibition, Supplemental Proceedings, Annual Meeting. 2013, The Minerals, Metals & Materials Society (TMS): Sydney, Australia: p. 301-309. 

[10] Xiong, D., Fang, K., Dai, X. and Luo, Y., Optimal Selection of Duck Density in Rice-duck Integrated Agro-ecosystems Based on Genetic Algorithm. Advances in Information Sciences and Service Sciences, 2013, 5(7): p. 1143-1156. 
