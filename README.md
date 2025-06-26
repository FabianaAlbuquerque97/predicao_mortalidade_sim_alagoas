# Predição de Mortalidade Infantil em Alagoas (2022-2025)

Este projeto tem como objetivo construir um modelo preditivo para estimar o risco de mortalidade infantil nos municípios de Alagoas, utilizando dados reais de nascimentos e óbitos infantis do ano de 2022. A partir deste modelo, são simulados cenários para previsão da mortalidade infantil em 2025, explorando variáveis demográficas e socioeconômicas relevantes.

## Motivação

A mortalidade infantil é um importante indicador de saúde pública e qualidade de vida. Prever corretamente os riscos em diferentes municípios permite que políticas públicas sejam melhor direcionadas, otimizando recursos e salvando vidas.

## Dados Utilizados

- **Nascidos vivos em 2022 em Alagoas:** dados municipais com número de nascimentos.
- **Óbitos infantis (< 1 ano) em 2022:** com informações detalhadas sobre idade, sexo, raça, escolaridade da mãe, tipo de parto, peso ao nascer, entre outros.

## Metodologia

1. **Pré-processamento dos dados:** limpeza, transformação e agrupamento das variáveis relevantes por município.
2. **Criação do target:** indicador binário de ocorrência de óbito infantil em cada município.
3. **Balanceamento das classes:** uso da técnica SMOTE para corrigir desbalanceamento entre municípios com e sem óbito.
4. **Modelagem:** Random Forest Classifier com ajuste de hiperparâmetros via Grid Search.
5. **Avaliação:** métricas de acurácia, precisão, recall, F1-score, matriz de confusão e validação cruzada estratificada.
6. **Simulação:** ferramenta interativa para explorar cenários futuros em 2025 com base em parâmetros ajustáveis.

## Resultados

- Modelo com alta acurácia (> 99%) e equilíbrio nas métricas.
- Identificação das principais variáveis preditoras como peso ao nascer, tipo de parto e idade média.
- Simulação interativa para visualização do risco municipal projetado para 2025.

-------------------------------------------------------------------------------------------------------------------------------------------

Links das bases de dados:

Natalidade: http://tabnet.datasus.gov.br/cgi/deftohtm.exe?sinasc/cnv/nval.def

Mortalidade: https://opendatasus.saude.gov.br/dataset/sim/resource/9ade641a-1f25-40d9-b55b-cff7096eb5b4?


## Tecnologias

- Python 3.x
- Pandas, NumPy, scikit-learn, imblearn (SMOTE), matplotlib, ipywidgets

---
