# Stonelab Challenge - AP2 Inteligência Artificial

Atividade Prática 2 (2026/1) - Case B: Churn de Clientes. O projeto constrói um pipeline para prever churn de lojistas e gerar uma explicação curta, coerente e fiel aos dados para apoiar o time de retenção.

## Estrutura

```text
.
├── data/
│   ├── dataset-churn.csv             # dataset bruto
│   ├── dataset-churn-corrigido.csv   # dataset corrigido/intermediário
│   └── schema_churn.json             # dicionário de dados e domínios
├── notebooks/
│   └── stone_churn_clients.ipynb     # notebook principal
└── README.md
```

## Como executar

Abra `notebooks/stone_churn_clients.ipynb` no Google Colab e execute todas as células. O notebook tenta carregar os dados locais quando estiver rodando dentro do repositório; caso contrário, usa as URLs raw do GitHub, sem upload manual.

O ambiente-alvo é Google Colab. As células instalam ou importam as dependências necessárias para análise, modelagem e geração de texto.

## Conteúdo Do Notebook

- **4.1 Representação do conhecimento:** validação pelo schema, correção estrutural, imputação, padronização e one-hot encoding.
- **4.2 Análise exploratória:** distribuição de classes, visualizações por classe, correlações e hipóteses.
- **4.3 Modelagem preditiva:** Regressão Logística e Random Forest com `Pipeline`, validação cruzada estratificada, `GridSearchCV`, métricas e matriz de confusão.
- **4.4 Geração de texto:** abordagem por templates e abordagem LLM via Hugging Face/prompt engineering.
- **5 Avaliação da qualidade do texto:** rubrica de coerência, completude e fidelidade, tabela de avaliação e análise crítica.

## Referências E Uso De IA Generativa

- Codex/GPT foi usado para apoiar o planejamento, estruturação do notebook e redação inicial de explicações.

## Integrantes

- Leonardo Guimarães de Melo Brito
- Rita Louro Barbosa
- Yuiti Kaneiko Leite