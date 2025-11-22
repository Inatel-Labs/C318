# C318 - Análise de Sentimento de Reviews (Steam)

Este projeto compõe a etapa de Análise Exploratória (EDA) e Pré-processamento de Dados da disciplina de Tópicos Especiais II.

O objetivo é carregar um dataset de reviews de jogos, visualizar estatísticas (positivos vs negativos), gerar nuvens de palavras e limpar o texto para uso futuro em modelos de Machine Learning.

## 🛠️ Pré-requisitos

**Recomendado:** Python 3.10+. As dependências principais estão em `requirements.txt`.

Crie e ative um ambiente virtual (PowerShell no Windows):

```powershell
python -m venv .\venv
.\venv\Scripts\Activate.ps1
```

Instale as dependências:

```powershell
pip install -r requirements.txt
```
```bash
pip install pandas matplotlib seaborn wordcloud nltk
```

Observações:
- `warnings` é módulo da stdlib — não precisa instalar.
- Se preferir travar versões, edite `requirements.txt` e rode o comando acima novamente.

## 🚀 Como Executar

1) Gerar/confirmar dados processados (notebook 1)

- Abra o Jupyter / VS Code ou rode via linha de comando. Se usar VS Code, abra `notebooks/1_analise_exploratoria.ipynb` e clique em "Run All" (ou "Executar Tudo") no topo do notebook.

2) Rodar a modelagem (notebook 2)

- Interativo (VS Code / Jupyter): abra `notebooks/2_modelagem_classificacao.ipynb` e execute usando "Run All" novamente.

- Saídas esperadas: métricas (accuracy, classification report), matrizes de confusão plotadas e gráficos de comparação de acurácia entre modelos. As imagens serão salvas na pasta `images/`.

## Como interpretar os resultados importantes

- `Acurácia` — proporção geral de acertos; útil como visão geral, mas sensível a desbalanceamento.
- `Classification report` — mostra precision, recall, f1-score por classe. Para o objetivo do projeto (priorizar leitura de reviews negativos), foque em **recall da classe negativa** (minimizar falsos negativos).
- `Matriz de confusão` — verifique contagens de verdadeiros positivos/negativos e falsos positivos/negativos para analisar erros do modelo.

## Contato

Entre em contato conosco através dos e-mails de [Marcos](marcos.guerra@ges.inatel.br) ou [Bruna](bruna.bs@ges.inatel.br).

###### C318  -  Professor: Ricardo Augusto da Silva Junior