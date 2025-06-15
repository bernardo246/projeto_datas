# 📊 Análise de Cancelamento de Clientes

Este projeto realiza uma análise exploratória de dados para entender os principais fatores que influenciam o cancelamento de clientes de um serviço, com base em dados históricos. A análise considera aspectos como **forma de pagamento**, **interações com o suporte**, **experiência de onboarding** e **avaliação da plataforma**.

## 🗂️ Dataset

O projeto utiliza o arquivo `BaseCancelamento.xlsx`, que contém as seguintes colunas relevantes:

- `Cancelou`: Indica se o cliente cancelou o serviço.
- `Forma de Pagamento`: Boleto, Cartão ou Pix.
- `Interacoes_Suporte`: Número de interações com o suporte.
- `Avaliação_Suporte`: Nota dada ao suporte.
- `Experiencia_OnBoarding`: Avaliação da experiência de início de uso.
- `Avaliação_da_Plataforma`: Nota geral da plataforma.
- `Código_Cliente`: Removido para manter a privacidade.

## 🔍 Objetivos da Análise

- Identificar se existe correlação entre o cancelamento e as variáveis analisadas.
- Calcular o **Valor da Informação (VOI)** de cada variável para entender seu poder de distinção entre quem cancela e quem não cancela.
- Visualizar os dados com gráficos interativos (Plotly) para facilitar a interpretação.

## 📈 Análises Realizadas

### 1. Forma de Pagamento

- Gráfico de barras mostrando a distribuição de cancelamentos por tipo de pagamento.
- Cálculo da diferença percentual entre quem cancelou e quem permaneceu.
- VOI da variável: `Forma de Pagamento`.

### 2. Suporte

- Análise das **interações com suporte** e da **avaliação recebida**.
- Dois gráficos de barras: um para interações e outro para avaliações.
- Cálculo do VOI para ambas as variáveis.

### 3. Onboarding

- Análise da **experiência inicial** do cliente com o serviço.
- Gráfico de barras + cálculo do VOI por nível de experiência relatado.

### 4. Avaliação da Plataforma

- Gráfico de barras mostrando cancelamentos por nota dada à plataforma.
- Cálculo do VOI para essa avaliação.

## 📊 Valor da Informação (VOI)

O VOI é utilizado como uma métrica para quantificar a influência de cada variável no cancelamento. Ele é calculado como a soma das diferenças absolutas entre as proporções de cancelamento e não cancelamento para cada categoria de uma variável.

## 🛠️ Tecnologias Utilizadas

- Python 3.9
- Pandas
- Plotly Express
- Math (biblioteca padrão)
- Jupyter Notebook

## 🧪 Como Executar

1. Instale as dependências:
```bash
pip install pandas plotly openpyxl