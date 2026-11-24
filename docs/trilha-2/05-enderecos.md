# 5. Endereços transparentes e blindados

!!! question "A pergunta desta página"
    Qual a diferença entre um endereço transparente e um blindado, e o que cada um mostra?

*Tempo de leitura: 6 minutos · Última revisão: novembro de 2026*

## Cartão-postal e carta lacrada

Imagine duas formas de mandar uma mensagem pelo correio.

O **cartão-postal** viaja aberto. Qualquer pessoa que o segure no caminho consegue ler o que está escrito e ver quem o enviou e quem vai receber.

A **carta lacrada** viaja dentro de um envelope. O carteiro sabe que uma carta foi enviada, mas não lê o conteúdo.

Na Zcash, os dois jeitos existem:

- O **endereço transparente** é o cartão-postal. Funciona como no Bitcoin: os detalhes da transação ficam visíveis a todos.
- O **endereço blindado** é a carta lacrada. Os detalhes ficam protegidos por criptografia.

## O que cada tipo mostra

O que a blockchain deixa à vista depende do tipo de endereço de quem envia e de quem recebe:

| Transação | O que fica visível |
|---|---|
| **Transparente → transparente** | Endereços e valor, para todos |
| **Transparente → blindado** (chamado de "blindar") | O valor fica visível do lado de quem envia |
| **Blindado → transparente** (chamado de "desblindar") | O valor fica visível do lado de quem recebe |
| **Blindado → blindado** | Quem enviou, quem recebeu e o valor ficam protegidos |

Em todos os casos, a **taxa** da transação aparece, e o fato de que ela aconteceu continua registrado. O que muda é o que o caderno da praça deixa ler sobre as pessoas envolvidas.

!!! tip "Para guardar"
    Quanto mais a movimentação acontece **dentro do lado blindado**, mais proteção ela tem. As passagens entre os dois lados revelam informação, por isso é bom saber quando elas acontecem.

## A privacidade é uma escolha

Nada obriga ninguém a usar um tipo ou outro. Há quem use o endereço transparente por ser mais simples ou compatível com mais serviços, e há quem prefira o blindado pela proteção. O suporte a cada tipo varia entre carteiras e serviços, e isso muda com o tempo.

## Um recado dentro da carta: o campo de memorando

Quando se envia valores para um endereço blindado, é possível anexar um **memorando**: uma mensagem de texto curta, também protegida por criptografia, que só quem recebe consegue ler. Pense num bilhete dentro do envelope lacrado.

## Mostrar só o que você quer: a chave de visualização

Privacidade não significa que ninguém jamais possa ver nada. Quem tem um endereço blindado também pode gerar uma **chave de visualização**, que dá a outra pessoa o direito de **ver** as transações daquele endereço, **sem poder gastar o dinheiro**.

É como entregar a alguém de confiança uma cópia da chave da janela, e não a do cofre: ela pode olhar lá dentro, mas não pode mexer em nada. Assim, você decide **quem vê o quê**.

## Um endereço só, vários tipos

À medida que a Zcash evoluiu, passaram a existir mais de um tipo de endereço blindado. Para evitar que o usuário precise escolher entre eles, foi criado o **endereço unificado**: um único endereço que reúne os tipos disponíveis, e a carteira cuida do resto. Para a maioria das pessoas, isso significa que basta compartilhar um endereço só.

## E agora?

Já vimos o que a carta lacrada esconde. Na próxima página, vamos entender **como** isso é possível: como a rede consegue conferir que a transação está correta sem abrir o envelope.

---

**Anterior:** [4. O que é a Zcash e de onde veio](04-o-que-e-zcash.md) · **Próxima:** [6. Como a privacidade funciona](06-como-funciona.md)

## Fontes

- [Addresses and Value Pools in Zcash (documentação)](https://zcash.readthedocs.io/en/latest/rtd_pages/addresses.html): o que fica visível em cada tipo de transação, taxas e memorando.
- [Zcash Basics (documentação)](https://zcash.readthedocs.io/en/latest/rtd_pages/basics.html): endereços transparentes e blindados, privacidade opcional e chave de visualização.
- [Unified Addresses (Electric Coin Company)](https://electriccoin.co/blog/unified-addresses): endereço unificado.
