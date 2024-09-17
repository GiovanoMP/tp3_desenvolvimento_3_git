# Dashboard: Percentual de Hóspedes por Motivo da Viagem (1997-2002)

Este projeto desenvolve um **dashboard interativo** que permite explorar o comportamento de hóspedes na cidade do Rio de Janeiro entre **1997 e 2002**, categorizados por motivo da viagem: **Negócios**, **Convenção**, **Lazer**, e **Outros**. O objetivo é fornecer uma análise visual e interativa de como os motivos de viagem variaram ao longo dos anos, com a possibilidade de selecionar colunas e filtrar os dados por ano.

## Link para o Deploy
O projeto está disponível via Streamlit e pode ser acessado através do link:

[https://data-rio.streamlit.app/](https://data-rio.streamlit.app/)

## Objetivo e Motivação

O turismo é uma das principais fontes econômicas do Rio de Janeiro, sendo fundamental para o desenvolvimento de políticas públicas e estratégias de marketing. Este dashboard visa:

- **Analisar as tendências** de viagem por motivos como Negócios, Convenção, Lazer, e Outros ao longo dos anos.
- **Auxiliar no planejamento estratégico** para o setor de turismo, identificando picos sazonais e mudanças no comportamento dos turistas.
- **Fornecer uma ferramenta interativa** para visualizar os dados e gerar insights que podem apoiar a criação de políticas mais focadas no desenvolvimento econômico da cidade.

## Funcionalidades Principais

1. **Gráfico por Ano**: 
   - O usuário pode escolher um ano específico entre 1997 e 2002 e selecionar as categorias de interesse (Negócios, Convenção, Lazer, Outros) para visualizar a variação mensal.
   - O gráfico é gerado com base nas colunas selecionadas e nos meses de janeiro a dezembro.

2. **Gráfico Comparativo de Todos os Anos**:
   - Exibe a média anual de cada motivo de viagem em um gráfico de linhas comparativo.
   - Inclui uma análise detalhada das tendências observadas para cada categoria de viagem.

3. **Upload e Download de Dados**:
   - O usuário pode fazer o upload de arquivos CSV ou Excel contendo dados personalizados para análise.
   - O dashboard permite o download dos dados processados diretamente pela interface, facilitando o acesso aos dados já filtrados e modificados.

4. **Status de Implementação**:
   - Uma aba dedicada para detalhar as funcionalidades implementadas, com o status de cada uma delas.

## Fontes dos Dados

Os dados utilizados neste dashboard são fornecidos pela Prefeitura da Cidade do Rio de Janeiro através do portal **Data.Rio**:

- [Data.Rio - Percentual de Hóspedes](https://www.data.rio/documents/ae953be9d6ee4af6ad77c56f34f6370b/about)

**Nota**: Os dados de 1995 e 1996 foram excluídos da análise, pois consistem apenas em médias anuais, sem detalhamento mensal. A análise foi focada nos anos de **1997 a 2002** para garantir consistência nos dados e maior granularidade.

## Tecnologias Utilizadas

- **Python**: Linguagem de programação utilizada para o desenvolvimento do projeto.
- **Streamlit**: Biblioteca para criação de aplicativos de dados interativos.
- **Pandas**: Para manipulação e análise de dados.
- **Matplotlib**: Para geração de gráficos e visualizações.
- **Requests**: Para baixar arquivos de dados e imagens hospedados online.
- **Excel Files**: Os dados originais foram fornecidos em formato `.xls` e processados dentro da aplicação.

## Estrutura do Projeto

```bash
├── data/
│   └── 469.xls                # Arquivo Excel original com os dados de hospedagem
├── imagem/
│   └── imagem_rio.jpeg         # Imagem da logo utilizada no dashboard
├── src/
│   └── app.py                  # Código principal do aplicativo Streamlit
└── README.md                   # Este arquivo README explicativo
