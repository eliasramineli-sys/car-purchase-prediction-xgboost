# Previsão de Compra de Automóveis com XGBoost

Projeto acadêmico de Ciência de Dados — Módulo 39. O objetivo é analisar uma base de clientes e treinar um classificador XGBoost para estimar a propensão de compra de automóveis.

## Dataset

Arquivo `data/CARRO_CLIENTES.csv`, com 1.000 registros e as colunas `User ID`, `Gender`, `Age`, `AnnualSalary` e `Purchased` (alvo binário).

## Etapas realizadas

1. Inspeção de tipos e valores ausentes e remoção do identificador.
2. Codificação da variável `Gender` com LabelEncoder.
3. Análise de correlação.
4. Divisão estratificada em treino (70%) e teste (30%).
5. Treinamento com `XGBClassifier` e hiperparâmetros configurados.
6. Probabilidades de previsão e avaliação com diferentes limiares.
7. Métricas de classificação, matriz de confusão e importância das variáveis.

## Como executar

Requer Python 3.10+ (recomendado). Na raiz do repositório:

```bash
python -m venv .venv
```

Ative o ambiente no Windows (PowerShell):

```powershell
.\.venv\Scripts\Activate.ps1
```

Instale as dependências:

```bash
pip install -r requirements.txt
jupyter notebook
```

Abra `notebooks/atividade_modulo_39_xgboost.ipynb` e execute as células na ordem. O caminho do CSV foi ajustado para funcionar a partir da pasta `notebooks/`.

## Organização

```text
car-purchase-prediction-xgboost/
├── data/
│   └── CARRO_CLIENTES.csv
├── notebooks/
│   └── atividade_modulo_39_xgboost.ipynb
├── .gitignore
├── requirements.txt
└── README.md
```

## Observações

Os resultados numéricos devem ser verificados executando o notebook no ambiente local. Trata-se de um exercício educacional, não de um modelo validado para uso em produção.

## Autoria

Projeto desenvolvido como atividade de formação em Ciência de Dados.
