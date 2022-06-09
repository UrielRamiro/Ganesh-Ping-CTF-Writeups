# Noite 5
O texto do challenge nos diz:
>Os presos estão reunidos no pátio de alimentação, você vê do alto uma movimentação atípica: os presos estão passando por baixo da mesa um prato. Você ordena que um guarda te traga. Em suas mãos está um prato de sopa de letrinhas estragado, de forma que as letras não se movem pelo caldo enrijecido. Você lê a seguinte mensagem:
```
Lsbok ib gmogds qdnggro, vsxxwa p LMN se kips usaak oreko t faejee orojrpdgg p ngwie
```
Novamente, a preseça de poucas vogais, nos remete que isso se da por uma cifra de substituição, usaremos novamente a mesma [ferramenta](https://www.dcode.fr/cipher-identifier) para analisar a cifra, vemos que tem boas chances de ser uma cifra de vigenere.

Utilizando então um decodificador de vigenere com a chave sopa (dica da noite passada), temos o seguinte plaintext:
```
Temos um guarda conosco, deixem a LUZ de suas celas acesa e fiquem acordados a noite
```
Então submetemos a flag Ganesh{a_dica_eh_luz}, foi!
