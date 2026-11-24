# 6. Como a privacidade funciona

!!! question "A pergunta desta página"
    Como é possível provar que uma transação é válida sem mostrar os detalhes dela?

*Tempo de leitura: 8 minutos · Última revisão: novembro de 2026*

## O problema da carta lacrada

Na página anterior, vimos que o endereço blindado funciona como uma carta lacrada. Isso levanta uma dúvida natural: se ninguém abre o envelope, **como a rede sabe que a transação está correta?** Como ter certeza de que ninguém está gastando dinheiro que não tem, ou o mesmo dinheiro duas vezes?

A resposta é uma ideia chamada **prova de conhecimento zero**.

## Provar sem mostrar

Imagine que você precisa provar a um porteiro que é maior de idade, mas sem mostrar sua data de nascimento, seu nome nem seu documento. Ele só precisa de uma coisa: a **certeza** de que a condição é verdadeira.

Uma prova de conhecimento zero faz exatamente isso: permite que uma pessoa convença outra de que uma afirmação é verdadeira, **sem revelar nada além do fato de que ela é verdadeira**.

Esse conceito foi criado por pesquisadores em 1985 e tem três características:

- **Convence quando é verdade.** Se a afirmação é verdadeira, quem sabe a resposta consegue demonstrá-la.
- **Não convence quando é falsa.** Quem não sabe a resposta não consegue enganar quem confere, a não ser com chance minúscula.
- **Não revela nada além do fato.** Quem confere não aprende mais nada.

!!! note "Uma história clássica: a caverna de Ali Babá"
    Uma caverna tem formato de anel, com uma entrada de um lado e uma porta mágica do lado oposto, que só abre com uma palavra secreta. Peggy afirma conhecer a palavra. Ela entra por um dos dois caminhos, sem que Victor veja qual. Então Victor grita por qual lado ela deve sair. Quem conhece a palavra sai pelo lado pedido todas as vezes. Quem não conhece só acerta na sorte, com 50% de chance por rodada. Depois de 20 rodadas, a chance de acertar sempre sem saber a palavra é de cerca de uma em um milhão. Victor fica convencido sem nunca ter ouvido a palavra.

## O que são os zk-SNARKs

A Zcash usa um tipo específico de prova de conhecimento zero chamado **zk-SNARK**. O nome é uma sigla em inglês, e o que importa é entender duas qualidades dele:

- Ele é **curto e rápido de verificar**, o que permite que a rede confira muitas transações.
- Ele **não exige conversa de ida e volta**, como a de Peggy e Victor. A prova é entregue pronta, e qualquer pessoa pode conferi-la depois.

Na Zcash, a prova que acompanha uma transação blindada atesta, sem mostrar os detalhes, que ela está correta: quem gasta tem o direito de gastar, o valor que entra é igual ao que sai, e aquele dinheiro não foi gasto antes.

## Como se evita gastar duas vezes

Aqui entra o detalhe mais engenhoso. Nos endereços blindados, cada valor existe como um **registro lacrado**, que a rede enxerga como um selo, sem saber o que há dentro dele.

Quando alguém gasta esse valor, publica um **carimbo de gasto único** (chamado *nullifier*, em inglês). Esse carimbo é diferente para cada registro, e a regra da rede é simples: **se o mesmo carimbo aparecer duas vezes, a segunda tentativa é recusada**.

O ponto mais interessante é que o carimbo **não revela de qual registro veio**. A rede consegue impedir o gasto duplo sem saber qual valor foi gasto, nem de quem.

Em resumo, a rede confere três coisas sem abrir o envelope:

1. a **prova** diz que a transação é válida;
2. o **carimbo** garante que o valor não foi gasto antes;
3. os **selos** permitem que a rede acompanhe os registros sem ler o conteúdo.

## A cerimônia e o fim da necessidade dela

Os primeiros zk-SNARKs, como os usados no lançamento da Zcash em 2016, precisavam de uma etapa inicial chamada **cerimônia de configuração**, em que participantes geravam parâmetros que o sistema usaria depois. Ela reuniu várias pessoas, justamente para reduzir a necessidade de confiar em uma só.

Em 2019, o pesquisador Sean Bowe descobriu o **Halo**, uma forma de gerar provas de conhecimento zero **sem precisar dessa configuração inicial**. Os desenvolvimentos mais recentes da Zcash usam essa abordagem. É um avanço importante, porque reduz a confiança necessária no sistema.

## O que a criptografia protege, e o que ela não protege

A proteção da Zcash vale para o que está registrado na blockchain. Algumas informações continuam de fora desse escudo:

- o **fato** de que a transação aconteceu, e a **taxa** paga;
- o que passa pelo lado **transparente**, como vimos na página anterior;
- o que a própria pessoa **divulga**, como mostrar o seu endereço em uma rede social ou informar a uma corretora que ele é seu.

A privacidade de uma pessoa é, portanto, resultado de duas coisas: a proteção da tecnologia e os hábitos de quem a usa.

## E agora?

Já temos a base para entender o que é a Zcash e como ela funciona. Na próxima trilha, vamos para a prática: como criar e usar uma carteira.

---

**Anterior:** [5. Endereços transparentes e blindados](05-enderecos.md) · **Próxima:** [7. Carteira, passo a passo](../trilha-3/07-carteira.md)

## Fontes

- [Zero-knowledge proof (Wikipedia)](https://en.wikipedia.org/wiki/Zero-knowledge_proof): definição, propriedades, caverna de Ali Babá e história.
- [Zcash Basics (documentação)](https://zcash.readthedocs.io/en/latest/rtd_pages/basics.html): zk-SNARKs e privacidade na Zcash.
- [Orchard Book: Nullifiers](https://zcash.github.io/orchard/design/nullifiers.html): selos (note commitments) e carimbos de gasto (nullifiers).
- [Zcash (Wikipedia)](https://en.wikipedia.org/wiki/Zcash): o Halo e a cerimônia de lançamento.
