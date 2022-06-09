# Noite 1
O texto do challenge diz:
>Você é um diretor de um presídio e, para conseguir fazer as reformas necessárias, precisa provar que os presos estão tentando fugir e capturar o líder do motim. Todas as noites os presos se comunicam tramando escapar, seu objetivo é decriptar as conversas e descobrir o nome do líder.
>
>Nesta série de desafios, a flag de cada desafio é uma dica para o próximo, que será liberado após resolvê-lo.
>
>**Noite 1.** Em uma cela de um presídio desconhecido em um lugar esquecido, dois presos compartilham a mesma ala. Você é o único de prontidão. Em meio ao silêncio, você ouve estalar de um cano:
```
1_5__3_3__4_4__1_5__3_3__1_4__1_5

4_3__2_4__3_2

4_4__3_4__4_1__4_5__1_5__1_2__4_2__1_1__3_3__1_4__3_4__3_4__1_3__1_1__3_3__3_4

3_4__2_5__1_1__4_4__1_5__3_3__4_4__1_5__1_1__3_4__5_1__2_4__3_3__4_4__1_5__1_5__3_3__3_4__5_1__1_5
```
>ESSA CIFRA ESTÁ APENAS NO GITBOOK.

Olhando o gitbook encontramos uma cifra muito parecida com a que foi utilizada, o Polibyus square (ou knock code).

A cifra consiste em utilizar batidas em alguma superficie que faça som, para formar palavras, decodificando a primeira linha teremos:

```
1_5__3_3__4_4__1_5__3_3__1_4__1_5 = entende
```
1_5 na tabela do gitbook, vale por um "e",  3_3 por um "n" e assim vai. o plaintext decifrado ficara assim:
```
entende
sim
to quebrando o cano
ok atente ao vinte e nove
```
Algo que o challenge diz, é que:
>A flag está no fromato Ganesh{a_dica_eh_**}

Isso significa que precisamos de apenas dois digitos para substituir os asteriscos.

Submetemos a flag Ganesh{a_dica_eh_29}, foi!