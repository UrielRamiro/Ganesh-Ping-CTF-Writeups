# Noite 3
O texto do challenge nos diz:
>Em uma outra inspeção é achado outra mensagem:
```
esarremes␣oait␣eoasie␣m␣ismdo␣f.nooiret␣eradissrgaemdp␣tsapps␣aospu␣t␣␣mob␣oo,co␣␣ns␣reai␣r
```
De cara, sem nem mesmo colocar em um analisador de frequencia, podemos perceber que vogais e consoantes se repetem de maneira similiar, deixando bem claro que isso é uma cifra de transposição.

Então, iremos usar uma [ferramenta](https://www.dcode.fr/transposition-cipher) para quebrar a cifra automaticamente, colocando a nossa ciphertext em conjunto com a dica do challenge anterior, temos o seguinte plaintext:

os rebites estao a romper, precisamos de mais dos nossos pra fugir. atente ao meio do impar.

Colocamos então a flag Ganesh{atente_ao_meio_do_impar}, e foi!