# Pafuntilo, O Criptografo
O texto do challenge diz:
>Pafuntilo é o monge que vivia no templo das 9 colunas e sabe-se que além de criptógrafo ele amava o nome que tinha já que o usava para encriptar tudo. Ele deixou esta mensagem pra você:

Com o seguinte ciphertext:
```
aNNn5_{13TT5s0UR1}G40h5LePR
```
De cara pra ciphertext não temos muita ideia de qual seria a sua crifa, mas o texto nos da uma dica de que uma possivel chave seria "Pafuntilo".

Analisando o ciphertext, podemos observar que ele possui bastantes numeros, que podem estar substituidos como letras, então para sabermos se a cifra é de substituição ou de transposição, iremos [analisar a frequencia](https://www.dcode.fr/frequency-analysis) da cifra.

E então vemos que ele tem 55,5% de consoantes (contando com o 5 que pode ser um S em leet) e 37,1% de vogais(tambem contando com os numeros que podem representar consoantes em leet) e por fim 7,4% de caracteres especiais.

Como observado a cifra tem uma quantidade muit proxima de frequencia entre vogais e consoantes, então provavelmente ela deve ser uma cifra de transposição, Utilizando um [decodificador de cifra de trannsposição](https://www.dcode.fr/transposition-cipher) com a chave "pafuntilo" temos o seguinte cipher text:
```
Ganesh{TR4N5P051T10N_RUL35}
```
Submetemos a flag, e ela foi