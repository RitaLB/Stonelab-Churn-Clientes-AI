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
├── AGENTS.md                         # guia para próximos prompts e manutenção
└── README.md
```

## Como executar

### Opção recomendada: Google Colab

Abra `notebooks/stone_churn_clients.ipynb` no Google Colab e execute todas as células. O notebook tenta carregar os dados locais quando estiver rodando dentro do repositório; caso contrário, usa as URLs raw do GitHub, sem upload manual.

O ambiente-alvo é Google Colab. As células instalam ou importam as dependências necessárias para análise, modelagem e geração de texto.

### Opção local

Se quiser executar localmente, crie uma `venv` e instale as dependências principais:

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install pandas numpy matplotlib seaborn scikit-learn jupyter transformers torch accelerate sentencepiece
jupyter notebook
```

Depois abra `notebooks/stone_churn_clients.ipynb` e selecione o kernel da `.venv`.

## Conteúdo Do Notebook

- **4.1 Representação do conhecimento:** validação pelo schema, correção estrutural, imputação, padronização e one-hot encoding.
- **4.2 Análise exploratória:** distribuição de classes, visualizações por classe, correlações e hipóteses.
- **4.3 Modelagem preditiva:** Regressão Logística e Random Forest com `Pipeline`, validação cruzada estratificada, `GridSearchCV`, métricas e matriz de confusão.
- **4.4 Geração de texto:** abordagem por templates e abordagem LLM via Hugging Face/prompt engineering com `Qwen/Qwen2.5-0.5B-Instruct`, sem necessidade de token.
- **5 Avaliação da qualidade do texto:** rubrica de coerência, completude e fidelidade, comparação entre abordagens e análise crítica.

## Referências E Uso De IA Generativa

- Codex/GPT foi usado para apoiar o planejamento, estruturação do notebook e redação inicial de explicações.
- Hugging Face foi usado para carregar o modelo `Qwen/Qwen2.5-0.5B-Instruct` na etapa de geração de texto.

## Integrantes

- Leonardo Guimarães de Melo Brito
- Rita Louro Barbosa
- Yuiti Kaneiko Leite
