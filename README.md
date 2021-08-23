# Habilidades

- Buscar documentos no banco
- Usar filtros na busca
- Deletar documentos conforme filtro
- Contar documentos compreendidos nos filtros pedidos
- Inserir documentos no banco

---

# Instalação

- Clone o repositório
- Entre na pasta do repositório que você acabou de clonar
- Instale as dependências:
```bash 
  npm install
```

# Requisitos do projeto

Durante a execução do projeto, utilize _queries_ do mongo para retornar os valores pedidos nos requisitos.

Você deve criar uma pasta chamada `challenges` na raíz do projeto, contendo dentro dela arquivos no formato `desafioX.js` onde `X` é o número do requisito.

Dentro dos arquivos `desafioX.js`, **crie uma query** ou mais (se necessário), para retornar o que o requisito pede. 

- [x] 1 - Retorne a quantidade de documentos inseridos na coleção `voos`.

- [x] 2 - Retorne os 10 primeiros documentos com voos da empresa `AZUL`.

- [x] 3 - Retorne a quantidade de voos da empresa `AZUL`.

- [x] 4 - Retorne a quantidade de voos da empresa `GOL`.

- [x] 5 - Retorne o `vooId` do décimo ao décimo segundo documento da coleção `voos`.

- [x] 6 - Retorne apenas os campos `empresa.sigla`, `empresa.nome` e `passageiros` do voo com o campo `vooId` igual a `756807`.

- [x] 7 - Retorne a quantidade de voos em que o ano seja menor do que `2017`.

- [x] 8 - Retorne a quantidade de voos em que o ano seja maior do que `2016`.

- [x] 9 - Retorne a quantidade de voos entre os anos de `2017` e `2018`.

- [x] 10 - Retorne apenas os **10** primeiros documentos com voos da empresa `GOL` do ano de `2017`. Exiba apenas os campos `vooId`, `empresa.nome`, `aeroportoOrigem.nome`, `aeroportoDestino.nome`, `mes` e `ano`.

- [x] 11 - Retorne a quantidade de documentos em que o campo `aeroportoDestino.pais` não seja igual a `ESTADOS UNIDOS`.

- [x] 12 - Retorne a quantidade de documentos em que o campo `aeroportoDestino.pais` seja igual a `BRASIL`, `ARGENTINA` ou `CHILE`.

- [x] 13 - Retorne a quantidade de documentos em que o campo `aeroportoDestino.continente` não seja igual a `EUROPA`, `ÁSIA` e `OCEANIA`.

- [x] 14 - Retorne o total de voos em que o país de origem não seja `BRASIL`.

- [x] 15 - Retorne o total de voos com mais de 20 `decolagens`.

- [x] 16 - Retorne o total de voos em que o campo `natureza` possui o valor `Internacional`.

- [x] 17 - Retorne o total de voos em que o campo `natureza` possui o valor `Doméstica`.

- [x] 18 - Retorne o `vooId`, `mes` e `ano` do primeiro voo com mais de `7000` passageiros pagos.

- [x] 19 - Retorne o `vooId` do primeiro voo em que o campo `litrosCombustivel` exista.

- [x] 20 - Retorne o `vooId` do primeiro voo em que o campo `rtk` não exista.

- [x] 21 - Retorne o `vooId` do primeiro voo em que o campo `litrosCombustivel` seja maior ou igual a `1000`.

- [x] 22 - Retorne o `vooId` do primeiro voo em que a empresa seja `DELTA AIRLINES` ou `AMERICAN AIRLINES`, a sigla do aeroporto de origem seja `SBGR` e a sigla do aeroporto de destino seja `KJFK`.

- [x] 23 - Retorne o `vooId` e `litrosCombustivel` do primeiro voo em que o campo `litrosCombustivel` **não seja maior do que** `1000` e o campo `litrosCombustivel` exista.

- [x] 24 - Retorne o `vooId`, `empresa.nome` e `litrosCombustivel` do primeiro voo em que `litrosCombustivel` **não seja maior do que** `600` **e** a empresa **não seja** `GOL` **ou** `AZUL`, **e** o campo `litrosCombustivel` exista.

- [x] 25 - Remova todos os voos da empresa `AZUL` em que a quantidade de combustível seja menor do que `400`. Informe a quantidade de documentos removidos.

- [x] 26 - Remova todos os voos da empresa `GOL` em que a quantidade de passageiros pagos esteja entre `5` e `10`, incluindo os casos em que a quantidade é `5` e `10`. Informe a quantidade de documentos removidos.

- [x] 27 - Retorne a quantidade total de voos de natureza `Doméstica` que a empresa `PASSAREDO` possui, via uso de uma nova coleção chamada `resumoVoos`.

Ou seja, a coleção `resumoVoos` conterá documentos onde cada um indica para cada empresa a quantidade total de voos que ela possui de natureza `Doméstica`.

Para isso, escreva no arquivo `desafio27.js` duas queries, **nesta ordem**:

1. Conte quantos voos da empresa `PASSAREDO` cujo campo `natureza` possua valor igual a `Doméstica` e crie uma query que insira na coleção `resumoVoos` um documento com os campos: `empresa` (nome da empresa) e `totalVoosDomesticos` (o total retornado anteriormente).

2. Em uma segunda query, retorne a `empresa` e o `totalVoosDomesticos` do primeiro documento presente na coleção `resumoVoos` em que a empresa seja `PASSAREDO`.

#### 28 - Retorne a quantidade total de voos de natureza `Doméstica` que a empresa `LATAM AIRLINES BRASIL` possui, via uso de uma nova coleção chamada `resumoVoos`.

Para isso, escreva no arquivo `desafio28.js` duas queries, **nesta ordem**:

1. Conte quantos voos da empresa `LATAM AIRLINES BRASIL` cujo campo `natureza` possua valor igual a `Doméstica` e crie uma query que insira na coleção `resumoVoos` um documento com os campos: `empresa` (nome da empresa) e `totalVoosDomesticos` (o total retornado anteriormente).

2. Em uma segunda query, retorne a `empresa` e o `totalVoosDomesticos` do primeiro documento presente na coleção `resumoVoos` em que a empresa seja `LATAM AIRLINES BRASIL`.

---
