# Stonelab Challenge — Case B: Churn de Clientes

Sistemas Inteligentes — Atividade Prática 2 (2026/1). Pipeline que prevê churn de lojistas e gera explicação em linguagem natural para a previsão.

## Estrutura

```
.
├── data/
│   └── churn_clientes.csv        # dataset (30 clientes)
├── notebooks/
│   └── stonelab_churn.ipynb      # notebook principal
└── README.md
```

## Como executar

Abra `notebooks/stonelab_churn.ipynb` no Google Colab e rode todas as células (Ambiente de execução → Executar tudo). O dataset é carregado automaticamente via URL raw do GitHub — não requer upload manual.

## Conteúdo

- **4.1** Representação do conhecimento (pré-processamento justificado)
- **4.2** Análise exploratória (EDA)
- **4.3** Modelagem preditiva — Regressão Logística e Random Forest, com validação cruzada e otimização de hiperparâmetros
- **4.4** Geração de texto — três abordagens: Templates, LLM (flan-t5) e Híbrida
- **5** Avaliação da qualidade do texto — rubrica humana e ROUGE-L

## Integrantes

_(preencher)_
