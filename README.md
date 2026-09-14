# 🚕 Zuber Chicago: Análise de Mobilidade & Teste de Hipóteses Estatísticas

## 📌 Contexto & Objetivo
A Zuber é uma nova empresa de compartilhamento de caronas que está sendo lançada em Chicago. O objetivo deste projeto é analisar padrões de mobilidade urbana, entender as preferências dos passageiros em relação às empresas de táxi/transporte e testar a hipótese estatística sobre o impacto das condições meteorológicas (dias chuvosos) na duração das corridas.

## 🛠️ Tecnologias e Ferramentas Utilizadas
- **Linguagem:** Python
- **Banco de Dados & Consultas:** SQL (PostgreSQL)
- **Análise & Estatística:** Pandas, NumPy, SciPy (`scipy.stats`)
- **Visualização de Dados:** Matplotlib, Seaborn
- **Ambiente:** Jupyter Notebook

## 🔎 Metodologia & Etapas
1. **Consultas SQL e Extração de Dados:**
   - Agrupamento de corridas por empresa de transporte para identificar os líderes de mercado.
   - Filtragem de bairros de destino mais populares em Chicago.
   - Junção de dados meteorológicos com registros de viagens para análise de impacto do clima.
2. **Análise Exploratória (EDA):**
   - Análise de distribuição dos bairros mais frequentes para desembarque.
   - Comparação da frota e volume de corridas das principais empresas da cidade.
3. **Teste de Hipóteses Estatísticas:**
   - **Hipótese Nula ($H_0$):** A duração média das corridas do Loop para o Aeroporto Internacional O'Hare nos sábados chuvosos é igual à duração em sábados ensolarados.
   - **Hipótese Alternativa ($H_1$):** A duração média das corridas nos sábados chuvosos é diferente da duração em sábados ensolarados.
   - Aplicação do **Teste T de Student para amostras independentes** (`scipy.stats.ttest_ind`).

## 📊 Principais Resultados & Insights
- Identificação dos bairros com maior concentração de desembarques, apontando regiões estratégicas para alocação de motoristas da Zuber.
- O teste estatístico confirmou relevância significativa ($p < 0.05$) na alteração do tempo médio de viagem em dias de chuva, fornecendo embasamento para precificação dinâmica e estimativa de tempo de chegada (ETA).

## 🚀 Como Executar o Projeto
1. Clone o repositório:
   ```bash
   git clone [https://github.com/derikpetiz/Zuber-Chicago.git](https://github.com/derikpetiz/Zuber-Chicago.git)
