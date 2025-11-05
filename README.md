# Análise de Músicas — Pipeline de Dados com Spotify API e NLP

Este projeto tem como objetivo **coletar, processar e analisar informações musicais** utilizando dados da **API Web do Spotify** e técnicas de **Processamento de Linguagem Natural (NLP)** aplicadas às letras das músicas.


## Objetivo

Criar um **pipeline completo de análise musical**, desde a coleta de dados de artistas e faixas até a extração de letras e análise de suas propriedades linguísticas, semânticas e de legibilidade.

O projeto busca responder perguntas como:
- Quais características diferenciam os gêneros musicais mais populares?  
- Como a linguagem das letras varia entre estilos como pop, rap, MPB e funk?  
- É possível detectar padrões linguísticos ou sentimentais relacionados ao sucesso de uma música?


## Etapas do Projeto

1. **Coleta de Dados**
   - Utilização da **API Web do Spotify** via biblioteca spotipy para obtenção de:
     - Gênero musical
     - Artista
     - Álbum
     - Popularidade

2. **Extração das Letras**
   - Uso de **web scraping** com requests e BeautifulSoup para buscar letras em fontes públicas como o site https://www.letras.mus.br.
   - Limpeza de textos com unidecode.

3. **Detecção e Pré-Processamento de Texto**
   - Detecção automática de idioma com langdetect.
   - Tokenização, remoção de stopwords e análise de estrutura linguística com nltk.

4. **Análise de Legibilidade e Métricas Textuais**
   - Avaliação de legibilidade com textstat e legibilidad.
   - Cálculo de indicadores como:
     - Comprimento médio de palavras
     - Número de sílabas por frase
     - Índice Flesch de leitura

5. **Modelos de Linguagem**
   - Integração de modelos da biblioteca **Transformers** (HuggingFace) para análise semântica e/ou classificação de sentimento.

6. **Visualização e Interpretação**
   - Criação de gráficos e comparativos entre gêneros, métricas linguísticas e popularidade.


## Tecnologias e Bibliotecas

- **Python 3**
- **Spotipy** - Acesso à API Web do Spotify  
- **Langdetect** - Detecção de idioma  
- **Transformers / Torch / Torchaudio** - Modelos de NLP  
- **Requests / BeautifulSoup4 / Unidecode** - Web Scraping e limpeza textual  
- **NLTK** - Processamento de texto e análise linguística  
- **Legibilidad / Textstat** - Métricas de legibilidade
- **Pandas / Matplotlib / Seaborn** - Organização e visualização dos resultados  

