# Aplicação de Machine Learning em Modelos de Credit Scoring

![Como Funciona a Concessão de Crédito](https://user-images.githubusercontent.com/97552106/221696744-d56739cc-7aab-465a-a78b-e2f7a3ee79bd.jpg)


## :dart: Objetivo
Desenvolver conhecimentos de Machine Learning aplicado no mercado Financeiro através do Curso de Machine Learning: Credit Scoring da Alura, com um case na Concessão de Créditos utilizando um dataset com informações reais do Banco Alemão Statlog (German Credit Data) extraídos do repositírio UCI. Como next steps, o objetivo é realizar ajustes deste modelo para obter uma melhor desempenho. 

## :bookmark: Contexto
Neste projeto, vamos entender como o Machine Learning também está inserido no mercado financeiro. A concessão de crédito faz parte da nosso dia-a-dia, como: cartões de crédito, empréstimos pessoais e consignados, financiamento de veículos e imobiliários, são apenas alguns dos exemplos de como o crédito está inserido na nossa rotina.

**Os 04 pilares da Cadeia de Créditos:**
- Prospecção;
- Concessão;
- Gestão de Risco;
- Recuperação;

Entretanto, o contexto deste projeto é voltado para: ***Concessão de Crédito***


**Credit Scoring**

Ou "Pontuação de Crédito" conforme sua tradução, é um modelo estatístico multivariado que cria um modelo matemático e estima, através de uma probabilidade, a chance do nosso cliente ser adimplente ou inadimplente. Dependendo da pontuação o tomador receberá o crédito para o empréstimo.

A Regressão Logistica é a técnica mais utilizada no sistema financeiro e a qual iremos utilizar para classificar os possíveis eventos: adimplentes ou inadimplentes. 

É importante que as empresas de cartão de crédito sejam capazes de reconhecer transações fraudulentas com cartão de crédito para que os clientes não sejam cobrados por itens que não compraram e não causarem prejuízos.

## :pushpin: Considerações do Dataset
Este conjunto de dados foi disponibilizado pelo Statlog (German Credit Data) dados reais, onde classifica as pessoas descritas por um conjunto de atributos como bons ou maus riscos de crédito.
- A Base de Dados disponibilizada já esta com as informações traduzidas conforme dicionário de dados disponibilizado;
- A Base de Dados contém ***informações sensíveis***, como o sexo da pessoa, a qual não deve ser considerado no modelo de acordo com as regulamentações do Banco Central.
- A variável `default` é a nossa variável resposta, onde: 0 = Credito Não Concedido | 1 = Crédito Concedido;

## :computer: Conteúdo
O Projeto foi organizados nos seguintes tópicos para uma melhor organização e compressão:
1. Sobre o Dataset do projeto e Análise Exploratória dos dados;
2. Transformação dos Dados
3. Declaração de Funções para os modelos;
4. Preparação dos dados de treino e teste;
5. Gerando o Modelo;
6. Gerando as Métricas;
7. Considerações Finais;

## :closed_book: Considerações Finais
Olhando para as métricas, podemos perceber que a acurácia, por exemplo, não é um bom parâmetro para avaliarmos o modelo que foi desenvolvido em cima de uma base de dados desbalanceados, isso porque os parâmetros do modelo não diferenciam a classe majoritária da minoritária. Através do cálcula da área ROC, obtivemos o valor de 0,764, que de acordo com a convenção estatística, temos uma discriminação aceitável.


## :bulb: Referências
[UCI Machine Learning](https://archive.ics.uci.edu/ml/datasets/statlog+(german+credit+data))
[Alura Cursos](https://cursos.alura.com.br/course/machine-learning-credit-scoring)
