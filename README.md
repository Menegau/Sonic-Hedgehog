# Sonic-Hedgehog

## O projeto

Este repositório será utilizado na disciplina de Aprendizado de Máquina. Os integrantes do trabalho são os alunos Alice Kageyama, Felipe Minatogau, Haziel Sanchez e Thaynara Matos.

Nosso trabalho durante essa disciplina será focado em desenvolver um programa que investiga a relevância das característicias físicas dos pinguins - tais como espécie, largura da nadadeira, profundidade e comprimento do bico, e entre outros - para a classificação de suas espécies, sendo estas o nosso target. 
Dessa maneira, o data frame utilizado tem como objetivo ajudar no nosso entendimento desde conceitos até a parte prática envolvida no apredizado de máquina.

## Organização 

Este projeto será organizado em algumas seções. A função deste tópico é facilitar a navegação nele.
A divisão será feita em pastas, cada uma com a identificação do seu respectivo bloco. 
Nessas pastas, estarão as tarefas realizadas por cada integrante, cuja identificação e contribuição podem ser visualizadas através dos *commits*. 

### Blocos
  #### No Bloco 1 - Obtenção e análise de dados -, os dados do DataFrame escolhido foram tratados da seguinte maneira: 
  
	1) Eliminamos espaços sem dados;
	2) Agrupamos os features numéricos;
	3) Normalizamos os dados para facilitar seu uso
	4) Descrevemos alguns fenômenos que ocorrem nos dados, tais como skewness (assimetria) e kurtosis (curtose - achatamento da curva de função de distribuição de probabilidade);
	5) Plotamos gráficos referentes aos dados analisados e à sua distribuição;
	6) Finalmente, citamos as fontes utilizadas.
  
  #### No Bloco 2 - Aprendizado Supervisionado -, os dados foram separados em gurpos para treino e para teste. Os métodos abordados foram os seguintes:
  
	1) k-NN (Nearest Neighbors ou vizinhos mais próximos);
	2) Regressão Linear;
	3) Árvore de decisão; 
	4) RandomForest (Floresta Aleatória);
  
	Após o estudo desses 4 métodos, realizamos a comparação entre eles, a fim de observar e avaliar o melhor resultado. Com isso, realizamos mais uma classíficação, afim de escolhermos os hiperparâmetros a serem utilizados no modelo de melhor resultado.  
  
  #### No Bloco 3 - Aprendizado Não Supervisionado -, foram utilizados algoritmos para analisar e clusterizar (agrupar/aglomerar) os dados não rotulados, para, dessa forma, eles encontrarem padrões por conta própria.
  
	1) O primeiro passo, foi a redução da dimensionalidade dos dados, através do método PCA, ou Principal Component Analysis;
	2) Após isso, foi realizada a clusterização dos dados através do método k-means;
	3) Além do k-means, um outro método a nosso critério foi escolhido, o "Clustering Hierárquico".

	Com os *clusters* definidos, utilizamos métodos para detectar os *outliers* (indivíduos ou dados fora do comum) no DataFrame. Para isso, foram aplicados os seguintes métodos:
	
	1.1) Isolation forest;
	2.1) Local Outlier Factor (LOF).
	
#### No Bloco 4 - Validação Cruzada e Conclusão -, foi utilizada a técnica de validação cruzada, a fim de avaliar os modelos utilizados nos blocos anteriores. Essa técnica consiste em comparar a aprendizagem dos algoritmos através da divisão dos dados em dois segmentos, os quais serão responsáveis por treinar o modelo e o outro para validá-lo.
	A validação foi realizada por meio do método k-fold, o qual, ao invés de apenas um treino, realiza vários k treinos. Em suma, o modelo em questão será treinado e testado um número k de vezes.
	Além disso, com o final da disciplina de Aprendizado de Máquinas, foi necessário conferir o repositório como um todo, a fim de encontrar erros tanto nos arquivos ReadMe quanto nos códigos. Em conjunto a isso, também julgamos necessário chegar a uma conclusão sobre qual o modelo que chegou em melhores resultados de previsão do nosso target em questão, isto é, a espécie dos pinguins. 

  
## Objetivos

Inicialmente, a meta definida era encontrar o comprimento dos bicos dos pinguins, o que seria realizado por meio dos diversos parâmetros contidos no DataFrame extraído da biblioteca seaborn. 
No entanto, depois de alguns testes iniciais, decidimos mudar o target para a espécie de pinguim, como citado no início da apresentação. 
Esse novo target pode se provar mais útil e racional, visto que as espécies costumam ser um dado mais importante e mais previsível a partir dos outros dados do que o comprimento dos bicos dos pinguins.
Outros objetivos a serem procurados serão adicionados neste tópico.
