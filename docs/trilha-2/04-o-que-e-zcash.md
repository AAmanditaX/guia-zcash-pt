# 4. O que é a Zcash e de onde veio

!!! question "A pergunta desta página"
    O que é a Zcash, quem a criou e qual problema ela quer resolver?

*Tempo de leitura: 6 minutos · Última revisão: novembro de 2026*

## Voltando ao caderno da praça

Na [página 2](../trilha-1/02-blockchain-sem-jargao.md), vimos que uma blockchain é como um caderno exposto na praça, que todos podem ler para conferir que as contas fecham. E, na [página 3](../trilha-1/03-bitcoin-e-privado.md), vimos o custo disso: no Bitcoin, quem lê o caderno enxerga de onde veio cada valor, para onde foi e quanto era.

A pergunta que ficou foi: será possível um caderno em que todos conferem que as contas fecham **sem precisar ler os detalhes de cada pessoa**?

A **Zcash** é uma resposta a essa pergunta. Ela é uma criptomoeda (cuja sigla é **ZEC**) que permite fazer transações com os detalhes protegidos, de modo que a rede consiga verificar que tudo está correto sem ver quem enviou, quem recebeu e quanto foi.

## A ideia central: privacidade que você escolhe

Na Zcash existem dois tipos de endereço, e você decide qual usar:

- **Transparente:** funciona como no Bitcoin. Os detalhes da transação ficam visíveis a todos.
- **Blindado:** os detalhes (quem enviou, quem recebeu e o valor) ficam protegidos por criptografia.

Por isso se diz que a privacidade na Zcash é **opcional**. Quem quiser pode usar a Zcash de forma transparente, e quem quiser proteção usa os endereços blindados. Detalharemos isso na [próxima página](05-enderecos.md).

!!! note "Um esclarecimento importante"
    Mesmo numa transação blindada, o fato de que ela aconteceu continua registrado na blockchain. O que fica protegido são os detalhes dela.

## De onde ela veio

A história da Zcash começa em pesquisa acadêmica, e não em uma empresa:

- **2013.** Pesquisadores da Universidade Johns Hopkins, nos Estados Unidos (entre eles Matthew Green, Ian Miers e Christina Garman), desenvolvem o *Zerocoin*, uma proposta para dar privacidade a moedas digitais.
- **Anos seguintes.** Esse trabalho se junta ao de outros cientistas, de instituições como o MIT, o Technion (Israel) e a Universidade de Tel Aviv, que desenvolveram os **zk-SNARKs**, um tipo de prova matemática que permite provar que algo é verdadeiro sem revelar a informação em si. É isso que torna possível o caderno "conferível, mas não legível". Veremos como funciona na [página 6](06-como-funciona.md).
- **2016.** A Zcash é lançada em **28 de outubro de 2016**, com o desenvolvimento liderado por Zooko Wilcox, por meio de uma empresa criada para esse fim.

Do ponto de vista técnico, a Zcash foi construída a partir do código do Bitcoin, com as proteções de privacidade acrescentadas. Por isso ela se parece com ele em vários aspectos. Um deles é o limite de moedas: assim como o Bitcoin, a Zcash tem um máximo de **21 milhões de ZEC**.

## Quem cuida da Zcash hoje

A Zcash é um projeto de **código aberto**: qualquer pessoa pode ler o código, e não existe um único dono. Ao longo dos anos, diferentes organizações e equipes de desenvolvedores participaram do projeto, e esse cenário muda com o tempo.

Por isso, em vez de listar nomes que podem estar desatualizados, recomendamos consultar o [site oficial da Zcash](https://z.cash) para saber quem mantém o quê no momento.

## E agora?

Já sabemos o que é a Zcash e de onde ela veio. Na próxima página, vamos entender melhor a diferença entre os endereços transparentes e os blindados, que é onde a privacidade acontece na prática.

---

**Anterior:** [3. O Bitcoin é privado?](../trilha-1/03-bitcoin-e-privado.md) · **Próxima:** [5. Endereços transparentes e blindados](05-enderecos.md)

## Fontes

- [Zcash (Wikipedia)](https://en.wikipedia.org/wiki/Zcash): origem, lançamento, relação com o código do Bitcoin e limite de moedas.
- [Zcash Basics (documentação)](https://zcash.readthedocs.io/en/latest/rtd_pages/basics.html): tipos de endereço e privacidade opcional.
