# 2. A blockchain sem jargão

!!! question "A pergunta desta página"
    O que é uma blockchain, e por que ela costuma ser pública?

*Tempo de leitura: 6 minutos · Última revisão: novembro de 2026*

## Um caderno na praça

Imagine uma cidade pequena onde todo mundo concorda em usar um mesmo caderno de registros. Ele fica exposto na praça. Quando Ana paga 10 moedas a Bruno, alguém escreve uma nova linha: "Ana pagou 10 a Bruno".

Esse caderno tem três características curiosas:

- **Muita gente guarda uma cópia.** Se alguém tentar rasurar a própria cópia, as outras mostram que ele está mentindo.
- **Só se escreve no fim.** Não dá para voltar e apagar o que já foi anotado.
- **Todo mundo pode ler.** Quem passa pela praça confere se as contas fecham.

Uma **blockchain** funciona como esse caderno, só que digital, mantido por milhares de computadores espalhados pelo mundo, sem que um deles mande em todos.

## Por que "cadeia de blocos"?

O nome vem do jeito como o caderno é organizado. As anotações são agrupadas em **blocos**, como páginas. Quando uma página enche, ela é "fechada" com uma espécie de selo que depende de tudo o que está escrito nela e do selo da página anterior.

Por isso as páginas formam uma **cadeia**. Se alguém tentasse mudar uma linha antiga, o selo daquela página deixaria de bater, e o das seguintes também. A fraude apareceria na hora.

## O problema que isso resolve

Quando você faz um Pix, existe uma instituição central que mantém o registro e garante que o mesmo dinheiro não seja gasto duas vezes. Você confia nela para isso.

Numa blockchain, não existe esse "dono do caderno". As regras estão no próprio sistema, e a rede inteira confere cada anotação. É isso que permite um dinheiro digital sem depender de uma instituição central no meio.

## E onde ficam as moedas?

Uma moeda digital não é um arquivo guardado no seu celular. Ela é, na verdade, **uma anotação no caderno**: "este endereço tem tantas moedas".

O que você guarda na sua **carteira** são as **chaves**, que provam que você é a pessoa com direito de mexer naquela anotação. Pense numa chave de cofre: o dinheiro não está na chave, mas quem tem a chave abre o cofre.

!!! warning "Por isso a chave é tão importante"
    Quem controla as chaves controla o dinheiro. Se você perde as chaves, não há banco ou atendimento para recuperá-las. E se alguém as descobre, pode gastar o que é seu. Voltaremos a isso na [página sobre segurança](../trilha-3/09-seguranca.md).

## Por que ela costuma ser pública?

Aqui está o ponto mais importante para este guia. Para que **todos possam conferir** que ninguém está gastando o que não tem, o caderno precisa estar aberto. Sem isso, seria preciso confiar em alguém.

Na maioria das blockchains, como a do Bitcoin, isso significa que **cada transação fica visível para qualquer pessoa, para sempre**: de qual endereço saiu, para qual foi e quanto foi.

Transparência e confiança caminham juntas nesse desenho. Mas, como vimos na [primeira página](01-por-que-privacidade.md), um caderno aberto a todos também tem um custo: ele expõe a vida financeira de quem o usa.

!!! note "A pergunta que fica"
    Será possível ter um caderno em que todos conseguem conferir que as contas fecham, **sem precisar ver os detalhes de cada pessoa**? Essa é a pergunta que a Zcash tenta responder, e chegaremos nela na [página 4](../trilha-2/04-o-que-e-zcash.md).

Antes, na próxima página, vamos desfazer um equívoco comum: o de que o Bitcoin seria anônimo.

---

**Anterior:** [1. Por que a privacidade financeira importa](01-por-que-privacidade.md) · **Próxima:** [3. O Bitcoin é privado?](03-bitcoin-e-privado.md)
