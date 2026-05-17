
# 🧠 NLP *(Processamento de Linguagem Natural)* & Análise de Sentimentos

<br><br>

## Visão Geral

O pipeline de NLP deste projeto transforma grandes volumes de textos financeiros em insights analíticos estruturados.

<br><br>

## Definição Técnica

**NLP (Natural Language Processing — Processamento de Linguagem Natural)** é uma área da Inteligência Artificial (IA) focada em permitir que máquinas compreendam, interpretem e processem linguagem humana.

**Análise de Sentimentos (Sentiment Analysis)** é uma subárea do NLP que identifica a polaridade emocional em textos, classificando-os como positivos, negativos ou neutros, além de detectar padrões de sentimento em grandes conjuntos de dados.

<br><br>

## Tecnologias

O projeto utiliza uma combinação de bibliotecas de NLP e ferramentas de processamento distribuído:

- **NLTK** *(Natural Language Toolkit — biblioteca fundamental para pré-processamento linguístico e pesquisa em NLP)*  
- **spaCy** *(framework de NLP de alta performance projetado para pipelines de produção)*  
- **PySpark NLP** *(framework de NLP distribuído baseado em Apache Spark para processamento escalável de texto)*  
- **TF-IDF** *(método estatístico para medir a relevância de termos em um corpus)*  

<br><br>

## Aplicação neste Projeto

O pipeline de NLP é aplicado em múltiplas fontes de dados financeiros:

- artigos financeiros  
- notícias sobre FIIs/REITs  
- postagens em redes sociais (tweets)  
- conteúdos de marketing financeiro  

<br><br>

## Objetivos

O sistema foi projetado para:

- identificar padrões de sentimento em textos financeiros  
- detectar tendências de mercado emergentes  
- extrair palavras-chave relevantes  
- gerar insights acionáveis de marketing  

<br><br>

## Exemplo

```python
text = "REITs mostraram forte valorização"
````

<br><br>



# 🧩 Divisão das Bibliotecas NLP

<br><br>

## NLTK *(Natural Language Toolkit — Kit de Ferramentas para Linguagem Natural)*

NLTK é uma biblioteca Python amplamente utilizada para pesquisa e educação em Processamento de Linguagem Natural.

**Definição Técnica:**
NLTK é uma biblioteca Python projetada para linguística computacional e tarefas de NLP.

**Propósito:**

* pré-processamento de texto
* tokenização
* remoção de stopwords
* stemming e lemmatization
* fundamentos de análise de sentimentos

**Papel neste projeto:**
Usado para limpeza e preparação de dados textuais brutos.

<br><br>

## spaCy *(Processamento de Linguagem Natural Industrial em Python)*

spaCy é um framework de NLP rápido e eficiente, otimizado para ambientes de produção.

**Definição Técnica:**
spaCy é uma biblioteca open-source de NLP focada em pipelines escaláveis e de nível industrial.

**Propósito:**

* Named Entity Recognition (**NER — Reconhecimento de Entidades Nomeadas**)
* análise de dependência e estrutura linguística *(análise sintática e estrutural)*
* tokenização
* POS tagging *(Part-of-Speech tagging — classificação gramatical das palavras)*
* extração de palavras-chave

**Papel neste projeto:**
Usado para extrair entidades financeiras estruturadas e informações semânticas de textos não estruturados.

<br><br>

## PySpark NLP *(Processamento Distribuído de Linguagem Natural)*

PySpark NLP é um framework de NLP construído sobre o Apache Spark para processamento distribuído em larga escala.

**Definição Técnica:**
PySpark NLP combina o poder do Apache Spark com pipelines de NLP para análise textual escalável.

**Propósito:**

* pipelines de NLP distribuídos
* análise de sentimentos em larga escala
* processamento massivo de textos
* embeddings *(representações vetoriais de texto)*
* modelos transformer *(arquiteturas de deep learning para linguagem natural)*

**Papel neste projeto:**
Permite processamento paralelo de grandes volumes de dados financeiros, como notícias e redes sociais.

<br><br>

## TF-IDF *(Term Frequency – Inverse Document Frequency)*

TF-IDF é uma técnica estatística usada para medir a importância de palavras em um conjunto de documentos.

**Definição Técnica:**
TF-IDF avalia a relevância de um termo comparando sua frequência em um documento com sua frequência em todo um **corpus** *(conjunto estruturado de textos usado para análise)*.

**Propósito:**

* extração de palavras-chave
* vetorização de texto
* engenharia de atributos para Machine Learning (ML)
* cálculo de relevância

**Papel neste projeto:**
Ajuda a identificar termos financeiros importantes no corpus de dados e melhora modelos de sentimento e classificação.


