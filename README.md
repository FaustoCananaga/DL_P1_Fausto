## Visão Geral do Projeto: Classificação de Imagens MNIST com Keras

Este notebook demonstra uma tarefa simples de classificação de imagens utilizando uma Rede Neural Convolucional (ConvNet), desenvolvida com Keras. O objetivo é classificar dígitos manuscritos do conjunto de dados MNIST.

### Enunciado do Problema

O problema abordado é a classificação de imagens em tons de cinzento de dígitos manuscritos (0–9). Esta é uma tarefa fundamental em visão computacional e é frequentemente utilizada como um exemplo introdutório ("Hello World") de aprendizagem profunda.

### Conjunto de Dados

O projeto utiliza o **MNIST**, um grande conjunto de dados de dígitos manuscritos. Ele é composto por **60.000 imagens para treino** e **10.000 imagens para teste**. Cada imagem possui dimensões de **28 × 28 píxeis** e está em escala de cinzentos.

### Como Executar

1. **Configuração do Ambiente:**
   Certifique-se de ter um ambiente Python com o Keras instalado. O notebook está configurado para utilizar o **TensorFlow como backend do Keras**. Pode executar as células iniciais para instalar os pacotes necessários e configurar o backend do Keras.

2. **Definição do Modelo:**
   O notebook define um modelo ConvNet sequencial utilizando `keras.layers`.

3. **Carregamento e Pré-processamento dos Dados:**
   O conjunto de dados MNIST é carregado diretamente através do Keras, redimensionado para incluir uma dimensão correspondente ao canal da imagem e normalizado para um intervalo entre **0 e 1**.

4. **Compilação do Modelo:**
   O modelo é compilado utilizando o otimizador `adam`, a função de perda `sparse_categorical_crossentropy` e a métrica `accuracy` (acurácia).

5. **Treino do Modelo:**
   O modelo é treinado utilizando os dados de treino durante **5 épocas**.

6. **Avaliação do Modelo:**
   Por fim, o modelo treinado é avaliado utilizando o conjunto de teste para determinar a sua **acurácia de classificação**.

