# challenge-telecom-x-2


# 📊 Análise de Evasão de Clientes - TelecomX

Este projeto contém um notebook em Python para análise de evasão (*churn*) de clientes de uma operadora de telecomunicações.  
O objetivo é explorar os dados, entender padrões de cancelamento e preparar informações para futuros modelos preditivos.

## 📈 Sobre a análise
A análise foi realizada em etapas, utilizando a base de clientes com informações contratuais, de serviços e de faturamento.

1. **Pré-processamento dos dados**  
   - Leitura do arquivo CSV com registros de clientes.  
   - Remoção de valores ausentes na coluna-alvo (*Cancelou*).  
   - Salvamento da base tratada para uso posterior.

2. **Análise descritiva**  
   - Cálculo da proporção de clientes ativos e cancelados.  
   - Verificação de possível desequilíbrio de classes, relevante para modelos de classificação.

3. **Codificação de variáveis categóricas**  
   - Aplicação de *one-hot encoding* para transformar variáveis categóricas em numéricas.  
   - Remoção da primeira categoria de cada variável para evitar colinearidade.

4. **Matriz de correlação**  
   - Cálculo das correlações entre variáveis numéricas.  
   - Identificação de quais variáveis possuem maior relação com a evasão (*Cancelou*).  
   - Visualização com *heatmap* usando paleta de cores `viridis` para facilitar leitura.

**Principais percepções:**  
- Foi identificado um certo desequilíbrio entre clientes ativos e cancelados, o que indica a necessidade de técnicas específicas para balancear dados em modelos preditivos.  
- Algumas variáveis, como tipo de contrato e uso de determinados serviços adicionais, apresentaram correlação mais forte com o cancelamento.  
- A visualização gráfica ajuda a priorizar variáveis mais relevantes para análise preditiva.

## 📦 Requisitos
```bash
pip install pandas seaborn matplotlib


📍 Autor: Seu Thiago Moura
📅 Última atualização: Agosto/2025



