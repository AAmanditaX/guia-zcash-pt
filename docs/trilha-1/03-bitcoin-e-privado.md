# 3. O Bitcoin é privado?

!!! question "A pergunta desta página"
    Muita gente acha que o Bitcoin é anônimo. Isso é verdade?

*Tempo de leitura: 6 minutos · Última revisão: novembro de 2026*

## O apelido no fórum

Pense em alguém que participa de um fórum na internet com um apelido, como "gato_azul_72". Ninguém sabe o nome verdadeiro dessa pessoa. Mas todas as mensagens ficam guardadas e ligadas ao mesmo apelido.

Basta um deslize, como mencionar a rua onde mora, postar uma foto ou usar o mesmo apelido em outro site, para que alguém ligue o apelido à pessoa. E, a partir daí, **todo o histórico** passa a ter dono.

No Bitcoin, os endereços funcionam como esse apelido. Chamamos isso de **pseudonimato**, e não de anonimato.

## O que o próprio Bitcoin promete

O texto que apresentou o Bitcoin ao mundo, o artigo de Satoshi Nakamoto de 2008, trata da privacidade de um jeito específico. Ele diz que a privacidade é mantida deixando as chaves públicas anônimas: qualquer pessoa vê que um valor foi de um endereço a outro, mas nada nesses endereços diz quem são as pessoas por trás deles.

O artigo compara isso ao que acontece na bolsa de valores, onde o horário e o tamanho de cada negociação são públicos, mas sem dizer quem foram as partes.

Ele recomenda ainda usar um endereço novo a cada transação, para que elas não sejam ligadas a um mesmo dono, e reconhece que **alguma ligação continua inevitável** quando uma transação reúne vários valores de entrada, porque isso revela que eles pertencem ao mesmo dono.

Ou seja, a privacidade no Bitcoin sempre dependeu de que **ninguém consiga ligar o endereço a uma pessoa**.

## Como o apelido vira nome

Na prática, essa ligação é feita com frequência, por vários caminhos:

- **Reuso de endereços.** Quem usa o mesmo endereço várias vezes junta, num só lugar, todo o seu histórico.
- **Pistas nas próprias transações.** Pesquisadores descrevem uma regra de bolso usada por quem analisa a blockchain: quando vários valores são gastos juntos numa mesma transação, assume-se que os endereços de origem pertencem à mesma pessoa. Repetindo isso, formam-se "grupos" de endereços ligados a um mesmo dono. Não é uma certeza, mas, num estudo de 2016, os autores mostraram que o método funciona surpreendentemente bem.
- **Pontos de contato com o mundo real.** Quando alguém compra ou vende em uma corretora que pede documentos, existe um registro que liga a conta (e os endereços usados nela) a uma pessoa. Quem identifica os endereços de uma corretora consegue reconhecer quem deposita e quem retira ali.
- **Informações públicas.** Um endereço divulgado em uma rede social, num pedido de doação ou numa loja pode bastar para ligar o apelido à pessoa.

Existem empresas especializadas nesse tipo de análise, e as técnicas continuam evoluindo.

## O detalhe que pesa: o caderno é permanente

Lembra da blockchain como um caderno na praça, em que nada se apaga? Esse é o ponto delicado. Um registro feito hoje **continua lá amanhã e daqui a dez anos**. Se, no futuro, alguém descobrir que determinado endereço é seu, todo o passado desse endereço se torna legível, inclusive transações que você fez quando achava que ninguém ligaria uma coisa à outra.

!!! note "Resumindo"
    Bitcoin **não** é anônimo. Ele é pseudônimo, e a privacidade que oferece depende de cuidado constante do usuário e de que ninguém conecte seu endereço à sua identidade. Quem sabe fazer isso direito consegue reduzir as ligações, mas o padrão é transparente.

## Por que isso importa para o resto do guia

Na primeira página, vimos por que a privacidade financeira importa. Aqui vimos que, no Bitcoin, ela depende de um esforço difícil e frágil. A pergunta natural é: **dá para construir um dinheiro digital em que a privacidade seja parte do funcionamento, e não um cuidado extra do usuário?**

É isso que a Zcash se propõe a fazer. Na [próxima página](../trilha-2/04-o-que-e-zcash.md), vamos conhecer a Zcash.

---

**Anterior:** [2. A blockchain sem jargão](02-blockchain-sem-jargao.md) · **Próxima:** [4. O que é a Zcash e de onde veio](../trilha-2/04-o-que-e-zcash.md)

## Fontes

- Satoshi Nakamoto, *Bitcoin: A Peer-to-Peer Electronic Cash System* (2008), seção 10, "Privacy". Texto reproduzido em [HackerNoon](https://www.hackernoon.com/bitcoin-white-paper-10-privacy-ex5232b7o).
- Martin Harrigan e Christoph Fretter, [*The Unreasonable Effectiveness of Address Clustering*](https://ar5iv.arxiv.org/html/1605.06369) (2016).

