# Neural Network SMS Text Classifier - Minha Solução

Solução em notebook para o projeto **Neural Network SMS Text Classifier** do freeCodeCamp.

## Conteúdo do ZIP

Este ZIP contém somente:

- `minha_solucao_sms_text_classifier.ipynb`
- `README.md`

Não foi incluído o notebook oficial/boilerplate do freeCodeCamp.

## Objetivo do projeto

Criar uma rede neural que classifique mensagens SMS como:

- `ham`: mensagem normal
- `spam`: propaganda, promoção, golpe ou mensagem automática

A função principal exigida é:

```python
predict_message(pred_text)
```

Ela retorna:

```python
[probabilidade, "ham" ou "spam"]
```

## Estratégia usada

A solução usa:

- TensorFlow/Keras
- `TextVectorization`
- vetorização `tf_idf`
- unigramas e bigramas com `ngrams=2`
- rede neural densa
- `Dropout`
- `class_weight` para compensar o desbalanceamento entre `ham` e `spam`
- escolha automática de limiar com balanced accuracy

## Como executar

1. Abra `minha_solucao_sms_text_classifier.ipynb` no Google Colab.
2. Execute as células em ordem.
3. O notebook baixará automaticamente os arquivos:

```text
train-data.tsv
valid-data.tsv
```

4. No final, a célula de teste deve exibir:

```text
You passed the challenge. Great job!
```

## Observação

O dataset não está dentro do ZIP porque o notebook baixa os dados diretamente pelo link oficial do freeCodeCamp.
