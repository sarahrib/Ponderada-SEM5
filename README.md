# Ponderada-SEM5

A partir da implementação da tradução automática, podemos responder às perguntas abaixo:

**1. Tente valores diferentes do argumento num_examples na funçãoload_data_nmt. Como isso afeta os tamanhos do vocabulário do idioma de origem e do idioma de destino?**
Quando mexemos no num_examples, temos uma resposta proporcional em relação ao tamanho do nosso vocabulário. Ou seja, quanto maior o num_examples, maior o nosso vocabulário se torna, e quando diminuimos, nosso vocabulários também reduz.

No texto foi testado 4 valores de num_examples e esses foram os resultados

**Exemplo 1**
num_examples = 100
vocabulários = 40

**Exemplo 2**
num_examples = 300
vocabulários = 102

**Exemplo 3**
num_examples = 600
vocabulários = 184

**Exemplo 4**
num_examples = 1000
vocabulários = 266



**2. O texto em alguns idiomas, como chinês e japonês, não tem indicadores de limite de palavras (por exemplo, espaço). A tokenização em nível de palavra ainda é uma boa ideia para esses casos? Por que ou por que não?**

Não, porque esses idiomas mais complexos e robustos, que não há separadores claros, como espaços, entre as palavras, o mesmo conjunto de caracteres pode ter significados diferentes dependendo do contexto. Por isso, a tokenização em nível de palavra pode não ser a melhor abordagem. É mais eficiente analisar os caracteres individualmente antes de determinar o significado final.
