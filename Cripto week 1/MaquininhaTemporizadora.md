# Maquininha Temporizadora
O texto do challenge nos diz:
>Um criptógrafo inventou uma máquina capaz de automaticamente encriptar mensagens que utilizam letras do alfabeto latino. Cada letra corresponde a um número (1 para A, 2 para B, …, 26 para Z). Além disso, algumas letras fazem parte de um conjunto especial (mantido em segredo), resultando em um comportamento especial da máquina.
>
>A máquina realiza a encriptação letra por letra, em dois passos, sendo que ambas as etapas levam o mesmo tempo (mesmo intervalo de tempo) para serem executadas:
>
> - Se a letra pertence ao conjunto especial, a máquina não realiza a encriptação, adiciona a letra original ao ciphertext e não executa o passo 2. Caso contrário, execute o passo 2.
> - Substitua a letra atual, associada a um número k, por uma letra y, onde y possui o mesmo resto ao dividir por 10 que k. Após isso, adicione a nova letra ao ciphertext.
Sabendo como a máquina funciona, decripte a seguinte mensagem:
```
Zkhubyds! U fbkg oh chifjyyhckssu.
```

e de acordo com a imagem sabemos quais caracteres do ciphertext não foram alterados, são eles: 5,8,10,13,15,16,18,23,26,27.

Deixaremos as letras maiusculas como sendo somente as que nós temos certeza de qual é o caractere certo.

```
zkhuBydS! u FbkG oH ChIfjyyHckSSu.
```
Agora montaremos uma tabela para as substituições dos caracteres com base nos modulos:

| %0 | %1 | %2 | %3 | %4 | %5 | %6 | %7 | %8 | %9 |
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
|  a |  b |  c |  d |  e |  f |  g |  h |  i |  j |
|  k |  l |  m |  n |  o |  p |  q |  r |  s |  t |
|  u |  v |  w |  x |  y |  z |    |    |    |    |

Tambem podemos apontar ao fato de que a cifra será poligrafica, assim que um simbolo se repetir, o proximo a baixo dele deverá ser utilizado, deixando o plaintext final dessa maneira:
```
PARABENS! A FLAG EH CRIPTOEHMASSA.
```
Inserindo a flag Ganesh{criptoehmassa} no challenge, foi!