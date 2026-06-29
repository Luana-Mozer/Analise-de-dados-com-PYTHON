# Analise de dados com PYTHON

Este projeto foi feito para praticar analise de dados com Python usando uma base de cancelamento de clientes.

A ideia foi entender quais fatores aparecem com mais frequencia entre os clientes que cancelaram o servico e transformar esses dados em informacoes mais claras para uma possivel tomada de decisao.

## Objetivo

Analisar uma base de clientes e identificar pontos que podem estar ligados ao cancelamento, como:

- tipo de contrato;
- quantidade de ligacoes para o call center;
- dias de atraso;
- perfil e comportamento de uso dos clientes.

## O que foi feito

No notebook eu segui um fluxo simples de analise:

1. importacao da base de dados;
2. visualizacao inicial das informacoes;
3. limpeza da base, removendo dados vazios e colunas que nao ajudam na analise;
4. analise da quantidade de clientes que cancelaram e que continuaram ativos;
5. criacao de graficos para comparar as colunas com o status de cancelamento;
6. aplicacao de filtros para simular possiveis acoes de reducao de cancelamento.

## Principais pontos observados

Durante a analise, alguns comportamentos chamaram atencao:

- clientes com contrato mensal tiveram maior cancelamento;
- clientes que ligaram muitas vezes para o call center tinham maior chance de cancelar;
- atrasos acima de 20 dias tambem apareceram como um ponto importante.

Com base nisso, testei filtros considerando contratos diferentes do mensal, ate 4 ligacoes para o call center e ate 20 dias de atraso. Apos esses filtros, a proporcao de cancelamento ficou menor na base analisada.

## Tecnologias usadas

- Python
- Pandas
- Plotly
- Jupyter Notebook

## Arquivos do projeto

- `analise.ipynb`: notebook com o passo a passo da analise.
- `cancelamentos.csv`: base de dados usada no projeto.
- `requirements.txt`: bibliotecas necessarias para executar o notebook.

## Como executar

1. Clone o repositorio:

```bash
git clone https://github.com/Luana-Mozer/Analise-de-dados-com-PYTHON.git
```

2. Entre na pasta do projeto:

```bash
cd Analise-de-dados-com-PYTHON
```

3. Instale as dependencias:

```bash
pip install -r requirements.txt
```

4. Abra o notebook:

```bash
jupyter notebook analise.ipynb
```

## Observacao

Esse projeto faz parte dos meus estudos em analise de dados com Python. O foco principal foi praticar limpeza de dados, leitura de indicadores e criacao de graficos para encontrar padroes dentro da base.
