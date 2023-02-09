# Conversor Monetário

## Desafio 2 - Conversor de Moedas com acesso a API REST

### Instruções
- A aplicação deve ser desenvolvida individualmente ou em dupla.
- Data limite de entrega: 18/01/2023 (quarta-feira).
- A aplicação deve ser versionada e disponibilizada no github.

### Descrição
Desenvolver uma aplicação modo texto (console) em C# que realize a conversão de
valores monetários entre diferentes moedas. A aplicação deve ler a moeda origem, a
moeda destino e um valor monetário e apresentar esse valor convertido da moeda
origem para a moeda destino e a taxa de conversão. Para realizar a conversão
propriamente dita deve ser consumido o serviço de conversão de moedas
exchangerate.

#### Serviço exchangerate
- [Documentação da API](https://exchangerate.host/#docs)
- URI de exemplo que converte o valor de USD 100,00 para reais https://api.exchangerate.host/convert?from=USD&to=BRL&amount=100.0

### Regras
- Moeda origem ≠ moeda destino.
- Moeda de origem e de destino devem ter exatamente 3 caracteres.
- Valor de entrada > 0.
- O valor convertido deve ser arredondado para 2 casas decimais.
- A taxa deve ser apresentada com 6 casas decimais.
- O programa deve terminar quando o usuário digitar string vazia para a moeda
  de origem.
- Erro na comunicação com a API: deve ser apresentada a mensagem de erro
  correspondente.
- Problemas na conversão: deve ser apresentada a mensagem de erro
  correspondente.