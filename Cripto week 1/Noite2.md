# Noite 2
O texto do challenge diz: 
>Vagarosamente pequenos estalos são ouvidos, devido ao estado de todo o pátio os barulhos são ignorados. Em uma inspeção rotineira um guarda acha um trapo com os seguintes dizeres:
```
r Vhqkru Hoxflgdgr dqgd shod qrlwh, pdv Qhp vhpsuh Kd Dojxhp.
```
Como um bom ganesher, você percebeu que a frequencia de consoantes é muito maior que a frequencia de vogais, então essa é uma cifra de substituição, mas não só isso se usarmos um [identificador de cifra](https://www.dcode.fr/cipher-identifier), ele irá nos mostra que isso provavelmente é uma cifra de cesar.

E como foi dito no texto do challenge anterior, cada flag do desafio é uma dica para o proximo, então a dica para esse challenge é 29, ficou obvio o que temos que fazer né?

movendo os caracteres 29 posições pra frente (ou melhor, 3 posições pra frente), temos o seguinte plaintext:
```
o Senhor Elucidado anda pela noite, mas Nem sempre Ha Alguem.
```
E é aqui que precisamos estar atentos, não é tão facil de perceber na primeira vez, mas há letrar em maiusculo que não deveriam estar em maiusculo, ordenando elas temos a palava
```
SENHA
```
Submetemos a flag Ganesh{a_dica_eh_senha}, foi!