# Projeto final - Modelo de Classificação para diabetes
---

Seja muito bem-vindo(a) ao repositório modelo-classificação-pima-projeto-final

## Sobre o projeto:
---

Este projeto é o trabalho final do curso [Scikit-Learn For Machine Learning Classification Problems](https://www.coursera.org/projects/scikit-learn-for-machine-learning-classification-problems), ministrado por Ryan Ahmed.

O objetivo, é criar um modelo de Aprendizado Supervisionado para classificação, que consiga apontar a positividade ou negatividade de diabetes para mulheres indianas da etnia Pima.

As aulas do curso são feitas em formato de projeto. O tema é doenças cardíacas, portanto é usado um dataset próprio.

Todos os conhecimentos adquiridos, tanto nas aulas, quanto na prática, estão sendo aplicados em um outro projeto meu [Aplicação web para Pré-Diagnóstico de Diabetes em Homens e Mulheres usando Aprendizado Supervisionado](https://github.com/rafaeldecastro195/modelo-classificacao-diabetes/blob/main/README.md)

## Sobre o dataset:
---

O dataset usado é [Diabetes Dataset - Pima Indians](https://www.kaggle.com/datasets/nancyalaswad90/review/data), disponível na plataforma do Kaggle.

Este possui `768 registros` e `9 atributos`:

| Atributo | Descrição | Tipo |
| :---: | :---: | :---: |
| **Pregnancies** | Número total de gestações | `int64` |
| **Glucose** | Taxa de glicemia | `int64` | 
| **BloodPressure** | Pressão arterial | `int64` |
| **SkinThickness** | Espessura da pele | `int64` |
| **Insulin** | Nível de insulina | `int64` |
| **BMI** | Índice de Massa Corporal (IMC) | `float64` |
| **DiabetesPedigreeFunction** | Função de Hereditariedade de Diabetes | `float64` |
| **Age** | Idade | `int64` |
| **Outcome** | Diagnóstico (`0` é negativo e `1`, positivo)| `int64` |

## Tecnologias utilizadas
---

| Nome | Descrição | Tecnologia de Origem|
| :---: | :---: | :---: |
| **Python** | Principal linguagem de programação para Ciência de Dados | `Python` |
| **Pandas** | Biblioteca de manipulação e análise de dados | `Python` |
| **Matplotlib** | Biblioteca de visualização de dados de maneira versátil | `Python` |
| **Seaborn** | Biblioteca de visualização de dados de maneira mais clara e elegante | `Python` |
| **Scikit-Learn** | Biblioteca de Aprendizado de Máquina, especialmente o Supervisionado | `Python` |
| **XGBoost** | Biblioteca de otimização de Aprendizado de Máquina, que usa conjuntos de árvores de decisão | `Python` |
| **Jupyter Lab** | IDE especializada em arquivos Jupyter Notebook (.ipynb) | `Jupyter Notebook` |
| **Git** | Sistema de versionamento de código, utilizado para enviar e versionar arquivos no repositório do GitHub | `Git` |

## Resultados do Modelo:
---

### Matriz de Confusão

| Predição | Performance | Percentual (%) |
| :---: | :---: | :---: |
| **Verdeiro Negativo** (TN) | 73 | 47.40 |
| **Falso Negativo** (FN) | 19 | 12.34 |
| **Verdeiro Positivo** (TP) | 36 | 23.38 |
| **Falso Positivo** (FP) | 26 | 16.88 |

***Notas***:
1. O total de predições no teste é `154`;
2. `Falso Negativo` é o erro mais sensível no contexto, já que o usuário teria a noção de que não está doente, mas na realidade estava, o que pode levar a um atraso do início do tratamento.

### Scores

| Métrica | Descrição | Classe 0 | Classe 1 |
| :---: | :---: | :---: | :---: |
| **Precision** | Proporção de predições corretas de uma classe |  0.79 | 0.58 |
| **Recall** | Capacidade do modelo em encontrar todos os casos reais da classe | 0.74 | 0.65 |
| **F1-Score** | Média harmônica entre Precision e Recall | 0.76 | 0.62 |
| **Support** | Quantidade real de ocorrências no conjunto de teste | 99 | 55 |

***Notas***:
1. A acurácia total do modelo é 0.71.

## Conclusões:
---

Trabalhar com Machine Learning é muito interessante. Contudo requer grandes conhecimentos em programação especializada, matemática e estatística.

Este é meu primeiro projeto na área e gostei muito. Indico o curso que fiz. Tive a oportunidade de aplicar:
- Análise Descritiva, por meio das Medidas de Tendência Central, visualização dos Histogramas (`Matplotlib`) e Matrizes de Correlação e Confusão (`Seaborn`).
- Análise Preditiva com o próprio Modelo de Classificação (`Scikit-Learn` e `XGBoost`).

O dataset utilizado é interessante, contudo é muito pequeno e específico, por ser de mulheres de uma etnia específica. Além disso, nele há uma feature de acesso mais difícil pelos usuários: a `DiabetesPedigreeFunction`. Acredito que estes fatores poderiam ser dificultadores de se levar o modelo a produção e à partir daí e, assim, criar uma aplicação que gere valor.

Pensando nisso, os conhecimentos adquiridos, tanto nas aulas do curso de Ryan Ahmed, quanto na prática e aplicação deste projeto, estão servindo de referência e sendo aplicados em um outro portfólio meu , chamado [Aplicação web para Pré-Diagnóstico de Diabetes usando Aprendizado Supervisionado](https://github.com/rafaeldecastro195/modelo-classificacao-diabetes/blob/main/README.md), que tem como objetivo a criação de uma plataforma web que determina, à partir dos dados das features, a probabilidade de o paciente ter diabetes mellitus, expressa em percentual. O intuito, é de a aplicação aconselhar o usuário, ao invés de diagnosticá-lo, o que é a competência dos profissionais da saúde. Neste projeto, uso outro dataset, significativamente maior, com features mais "triviais" para o usuário, além de englobar não somente o gênero feminino. Ainda em desenvolvimento.

## Agradeço a visita ao repositório!
