# Mini Projeto de Deep Learning usando TensorFlow

## Visão Geral do Projeto
Este mini-projeto demonstra um modelo de deep learning implementado usando TensorFlow. O modelo é treinado em um dataset diferente do apresentado em sala de aula. O projeto inclui métricas como acurácia, acurácia de validação, F1 Score e perda durante o treinamento e validação.

## Dataset
Utilizamos o **Fashion MNIST**, que contém imagens em escala de cinza de 10 diferentes tipos de roupas. Cada imagem tem 28x28 pixels, e o dataset possui 60.000 imagens de treinamento e 10.000 imagens de teste.

## Arquitetura do Modelo
O modelo é uma Rede Neural Convolucional (CNN) composta pelas seguintes camadas:
- **Conv2D**: 32 filtros, kernel de 3x3, ativação `ReLU`
- **MaxPooling2D**: pool size de 2x2
- **Conv2D**: 64 filtros, kernel de 3x3, ativação `ReLU`
- **MaxPooling2D**: pool size de 2x2
- **Dense**: 128 unidades, ativação `ReLU`
- **Camada de Saída**: ativação Softmax para 10 classes

## Métricas e Desempenho
O modelo foi avaliado utilizando várias métricas:
- **Acurácia**
- **Acurácia de Validação**
- **F1 Score**
- **Matriz de Confusão**

### Exemplo do Gráfico de Acurácia:
(Incluir gráfico de acurácia/perda aqui)

## Como Executar o Projeto
### Treinando o Modelo:
1. Clone este repositório.
2. Instale as dependências necessárias: `pip install -r requirements.txt`
3. Execute o notebook `train_model.ipynb` para treinar o modelo.

### Fazendo Previsões com o Modelo:
1. Use o notebook `predict_model.ipynb` para carregar os pesos salvos e realizar previsões nos dados de teste.
2. Os pesos do modelo estão salvos no arquivo `fashion_mnist_model.h5`.

## Estrutura do Repositório
- **predict_model.ipynb**: Notebook Jupyter para treinar o modelo, carregar os pesos do modelo e fazer previsões.
- **fashion_mnist_model.h5**: Pesos pré-treinados do modelo.
