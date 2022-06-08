# Literatura Inglesa
A mensagem do challenge diz:
>Esta mensagem foi encontrada no meio dos trabalhos de um grande e conhecido escritor da língua inglesa, mas infelizmente está criptografada. A flag é o nome do ser ao qual a quarta linha se refere. Insira a flag no formato Ganesh{flag_aqui}.

com o seguinte ciphertext:
```
VALYY LXPFK SQL VAY YCRYP IXPFK BPUYL VAY KIE,
KYRYP SQL VAY UONLS CQLUK XP VAYXL ANCCK QS KVQPY,
PXPY SQL GQLVNC GYP, UQQGYU VQ UXY,
QPY SQL VAY UNLI CQLU QP AXK UNLI VALQPY
XP VAY CNPU QS GQLUQL OAYLY VAY KANUQOK CXY.
QPY LXPF VQ LBCY VAYG NCC, QPY LXPF VQ SXPU VAYG,
QPY LXPF VQ MLXPF VAYG NCC NPU XP VAY UNLIPYKK MXPU VAYG.
XP VAY CNPU QS GQLUQL OAYLY VAY KANUQOK CXY.
```
Batendo o olho podemos ver que isso é claramente uma cifra de substituição e, de acordo com o challenge, está em inglês.

Iremos então [analisar a frequencia](https://www.dcode.fr/frequency-analysis) das letras do ciphertext e compara-las à [lista de frequencia da lingua inglesa](https://pt.wikipedia.org/wiki/Frequ%C3%AAncia_de_letras#Frequ.C3.AAncias_relativas_das_letras_na_l.C3.ADngua_inglesa).

Em ambas as tabelas a principal letra apresenta 3 pontos percentuais acima da segunda, provavelmente não se trata de uma anomalia estatistica, iremos então substituir Y por e, dado as duas frequencias, ficando então:
```
VALee LXPFK SQL VAe eCReP IXPFK BPUeL VAe KIE,
KeReP SQL VAe UONLS CQLUK XP VAeXL ANCCK QS KVQPe,
PXPe SQL GQLVNC GeP, UQQGeU VQ UXe,
QPe SQL VAe UNLI CQLU QP AXK UNLI VALQPe
XP VAe CNPU QS GQLUQL OAeLe VAe KANUQOK CXe.
QPe LXPF VQ LBCe VAeG NCC, QPe LXPF VQ SXPU VAeG,
QPe LXPF VQ MLXPF VAeG NCC NPU XP VAe UNLIPeKK MXPU VAeG.
XP VAe CNPU QS GQLUQL OAeLe VAe KANUQOK CXe.
```
e repetiremos o processo, mas levando em conta que podem haver anomalias estatísticas, como por exemplo o Q que é a segunda letra que mais se repete no ciphertext, porem ele só sera substituido pelo O que é a quarta letra que mais se repete na lingua ingles.

Ao decifrar boa parte do texto, é possivel identificar palavras pelo contexto e chegarmos ao plaintext:
```
three rings for the elven kings under the sky,
seven for the dwarf lords in their halls of stone,
nine for mortal men, doomed to die,
one for the dark lord on his dark throne
in the land of mordor where the shadows lie.
one ring to rule them all, one ring to find them,
one ring to bring them all and in the darkness bind them.
in the land of mordor where the shadows lie.
```
A flag do challenge é o nome do ser ao qual a quarta linha se refere, Ganesh{Sauron}.

Submit na flag, e foi.