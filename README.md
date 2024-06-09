# TP1 - Redes Neuronais + Backpropagation

## Informações do Projeto

- **Aluno**: Laisson Bruno dos Reis Germano
- **Professor**: Dr Adriano Alonso Veloso
- **Disciplina**: Aprendizado de Máquina
- **Programa**: UFMG - Programa de pós graduação em ciência da computação - Mestrado

## Descrição do Projeto

Neste trabalho, você irá implementar uma rede neural com três camadas para classificação de dígitos manuscritos utilizando o dataset MNIST. A rede neural será composta por:

1. **Camada de Entrada**: Cada unidade representa uma dimensão do dado de entrada.
2. **Camada Oculta**: Cada unidade representa uma transformação a partir das unidades de entrada.
3. **Camada de Saída**: Cada unidade representa a probabilidade da saída correspondente ser a correta.

## Especificações da Rede Neural

- **Função de Ativação**: Sigmóide para introduzir não-linearidade.
- **Função de Perda**: Cross Entropy, que será minimizada durante o treinamento.
- **Dados**: O dataset MNIST, contendo 5000 entradas, onde cada entrada refere-se a um dígito escrito manualmente. Cada entrada é uma matriz de 28x28 pixels, representada como um vetor de 784 dimensões. A primeira coluna do arquivo é o rótulo do dígito correto.

## Estrutura da Rede Neural

- **Unidades de Entrada**: 784
- **Unidades de Saída**: 10
- **Unidades na Camada Oculta**: Variar entre 25, 50 e 100

## Algoritmos de Cálculo de Gradiente

Você deverá comparar os seguintes algoritmos de cálculo de gradiente:

1. **Gradient Descent**: O gradiente é calculado após cada época (após as 5000 entradas serem processadas).
2. **Stochastic Gradient Descent**: O gradiente é calculado após cada entrada.
3. **Mini-Batch Gradient Descent**: O gradiente é calculado após um certo número de entradas (considere 10 e 50).

## Taxas de Aprendizado

Você deverá variar a taxa de aprendizado entre os seguintes valores: 0.5, 1, 10.

## Experimentos e Resultados

O documento a ser entregue deverá apresentar os resultados dos seus experimentos, incluindo:

- Discussão sobre a variação do número de unidades na camada oculta para cada um dos três algoritmos de cálculo de gradiente.
- Gráficos mostrando a convergência do erro empírico para cada situação (unidades na camada oculta, algoritmo de cálculo do gradiente, taxa de aprendizado).
- Hipóteses e considerações pertinentes.

## Ferramentas Recomendadas

Você pode utilizar pacotes que facilitam a implementação e treinamento de redes neurais, como PyTorch ou TensorFlow.