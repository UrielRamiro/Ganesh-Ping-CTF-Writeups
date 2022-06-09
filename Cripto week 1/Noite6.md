# Noite 6
O texto do challenge nos diz:
>Ao saber do guarda corrupto você ordena que um funcionário de confiança se passe por preso para pegar a mensagem. No meio da noite ele entra ofegante em seu escritório e te entrega um papel dizendo:
```
L ztgf mkrs lfjl, qxq q qmbq rbagc mh pajsaj v lafpzus r mcdhg, ps wzgsavfr gf tnhxo, tagifslb vrgnc ewgfvw Frvfid.
```
Novamente é possivel observar que se trata de uma cifra de substituição, utilizando o analisador de cifra ... dessa vez não vai funcionar, o identificador falha em acertar qual é essa cifra, só nos resta voltar ao gitbook ou as aulas do ganesh e tentar achar algo similiar a essa cifra, mas temos uma forte candidata, a cifra AutoKey.

Então ao testarmos descriptografar o ciphertext, com a chave luz que foi a dica do challenge anterior, temos o seguinte plaintext:
```
A fuga sera hoje, com o cano rompo as barras e liberto a todos, me encontre no patio, assinado vosso mestre Martim.
```
Submetemos a flag Ganesh{o_lider_eh_martim} e... NÃO FOI.

É... aqui temos um probleminha, a flag deveria ser martim, mas por algum motivo o certo é martin, com N, submetendo a flag Ganesh{o_lider_eh_martin}, agora sim, foi!