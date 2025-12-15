# Validação de modelos de clusterização para moderação de conteúdo

## Contexto

Este projeto foi desenvolvido na disciplina **Validação de modelos de clusterização [25E4_3]** do curso de pós-graduação em Inteligência Artificial.  
O objetivo é explorar técnicas de **clusterização de textos** para apoiar a moderação de conteúdo em mídias sociais.

## Objetivo

- **Objetivo de negócio:** reduzir a carga de revisão manual de textos classificados como “negativos”, priorizando aqueles com maior risco de ofensa.
- **Objetivo técnico:** utilizar embeddings (Sentence-BERT) e algoritmos de clusterização (K-Means, DBSCAN) para identificar grupos temáticos dentro da classe negativa e avaliar diferentes medidas de similaridade e métricas de validação.

## Dados

- Dataset: [`tweet_eval/sentiment`](https://huggingface.co/datasets/tweet_eval)
- Classes: 0 = negativo, 1 = neutro, 2 = positivo  
- O foco do projeto é a **classe negativa (0)**.

Os dados são carregados diretamente via HuggingFace no notebook, não há arquivos de dados versionados neste repositório.

## Ambiente e dependências

- Python 3.10+ (ou versão usada na disciplina)
- Bibliotecas listadas em `requirements.txt`

### Criar ambiente virtual (opcional, recomendado)

```bash
python -m venv .venv
source .venv/bin/activate  # Linux/Mac
# ou
.\.venv\Scripts\activate   # Windows

pip install -r requirements.txt
```
