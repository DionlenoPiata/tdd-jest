# TDD JEST

> TDD: Como criar unit tests em Node.js com Jest

## Executar aplicação

```sh
npm install
npm test
```

## Introdução ao TDD

O Test Driven Development/TDD ou Desenvolvimento Orientado à Testes é uma técnica criada por Kent Beck, um famoso programador e autor de livros que atualmente trabalha no Facebook. Também são de autoria de Beck a metodologia ágil Extreme Programming (XP) que inclui técnicas como o TDD e o Pair Programming, que já falei aqui no blog.

A ideia do TDD é que você deve escrever primeiro os testes da sua aplicação, para depois implementar o código que fará com que eles funcionem. Isso pode soar um tanto estranho mas é uma ideia ousada que possui vários benefícios, tais como:

diminuição do número de bugs, uma vez que não existem features sem testes;
foco nas features que importam para o projeto, pois escrevemos os testes com os requisitos em mãos;
permite testes de regressão, para ver se um sistema continua funcionando mesmo após várias mudanças e/ou muito tempo desde a última release;
aumento da confiança do time no código programado;
O TDD é executado em um ciclo chamado de Red/Green/Refactor e prega que cada incremento pequeno de software (baby step) deve ser testado, para que bugs sejam corrigidos rapidamente assim que surgem. Ele prega que primeiro você deve escrever o teste, antes mesmo da feature ser implementada. Quando executar esse teste, ele irá falhar (Red), aí você codifica a feature apenas o suficiente para ela passar no teste (Green) e então você melhora o código para que ele não apenas seja eficaz, mas eficiente (Refactor).

Recomenda-se rodar novamente os testes e se após a refatoração a feature parar de funcionar, roda-se o ciclo novamente.

O coração do TDD são os unit tests.
