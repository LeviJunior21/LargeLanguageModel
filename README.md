# Large Language Model

## Neste repositório encontra-se alguns dos passos básicos necessários para a criação de uma LLM.

### [FeedForward](./FeedForward.ipynb)
Neste notebook Google Colab eu tenho feito o FeedForward (propagação para frente) para um modelo que a partir de um contexto prever a próxima palavra usando o PyTorch.

### Transformer

Modelos de linguagem baseados em arquiteturas de Transformers revolucionaram o campo de Processamento de Linguagem Natural (PLN), permitindo avanços expressivos em tarefas como tradução automática, sumarização, resposta a perguntas e geração de texto. Entre esses modelos, o GPT-2 (Generative Pretrained Transformer 2), proposto pela OpenAI em 2019, destacou-se como um dos primeiros a demonstrar a capacidade de gerar texto coerente e contextualizado em larga escala.

A arquitetura do GPT-2 é composta por blocos de transformers decoders, que utilizam mecanismos de atenção para modelar dependências de longo alcance em sequências textuais. Dois elementos fundamentais para o funcionamento desse tipo de modelo são os embeddings posicionais, que permitem incorporar a noção de ordem das palavras, e o mecanismo de atenção multi-cabeças (Multi-Head Attention), responsável por capturar relações contextuais em diferentes subespaços de representação.

Nos últimos anos, diversas variações da arquitetura original foram propostas, buscando melhorar a eficiência computacional e a qualidade do modelo. Uma dessas variações é o Grouped-Query Attention (GQA), que reduz o custo da atenção agrupando consultas (queries), mantendo boa capacidade representacional ao mesmo tempo em que economiza memória e acelera a inferência.

Este trabalho tem como objetivo implementar, treinar e avaliar um modelo inspirado no GPT-2 do zero, utilizando um conjunto de textos em português de domínio público. Além da implementação do baseline, exploramos modificações arquiteturais, em particular:

O uso do embedding posicional da arquitetura original do GPT-2;

A implementação de Grouped-Query Attention (GQA).

A avaliação do modelo será realizada por meio de métricas quantitativas, como a perplexidade no conjunto de teste, além da análise de desempenho (tokens/s e consumo de memória). Também conduziremos uma análise qualitativa das gerações de texto, comparando o baseline com as variantes propostas.

Com isso, buscamos não apenas reproduzir parte do funcionamento do GPT-2, mas também compreender o impacto de modificações arquiteturais em termos de qualidade, eficiência e capacidade de generalização em língua portuguesa.
