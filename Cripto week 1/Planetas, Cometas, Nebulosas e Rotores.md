# Planetas, Cometas, Nebulosas e Rotores
O texto do challenge diz:
>A seguinte mensagem criptografada foi encontrada próxima a uma máquina Enigma, na casa de um famoso escritor que adorava refletir, em todas as suas obras, sobre as peculiaridades do Universo:
```
I XKOFEMBS JPLU Y FATF, S CUXAHLXH W LCKT XHDV É (CMOOPTZX G FMUV)
```
> Sabe-se que essa Enigma possuía apenas 2 rotores e 1 refletor, e ignorava todos os espaços, pontuações e caracteres especiais. O segundo rotor rotaciona a cada letra digitada e o primeiro rotor rotaciona a cada 26 rotações do segundo.
>
>Na tentativa de decriptar a mensagem, um criptólogo verificou a saída da máquina ao digitar a letra U (de Universo) utilizando várias posições distintas para os 2 rotores e disponibilizou o resultado no arquivo enigma.txt.
>
>Além disso, a fim de que mais pessoas auxiliassem em sua tarefa, ele desenvolveu um simulador em Python dessa máquina, disponibilizado no arquivo enigma.py, que permite encriptar/decriptar mensagens dada uma posição inicial para o primeiro rotor (localizado à esquerda) e para o segundo rotor (localizado à direita).

Para começar, a Enigma é uma cifra de Substituição, ou seja, não altera a ordem dos elementos, Então como a palavra Universo possui 8 letras, um bom chute seria utilizar essa informação para testar as 3 palavras com 8 letras do ciphertext, No caso, aqui escolheremos a segunda: "CUXAHLXH".

No challenge, nos é dado um enigma.py que é o algoritmo do enigma que será utilizado para a resolução do chal, e a enigma.txt que contem informações a respeito de qual letra vira qual em determinada posição do rotor.

Ao testar as posições de rotor na qual o U é trocado por C, chegamos na resposta de que quando o primeiro rotor está na posição 5 e o segundo rotor está na posição 3, a palavra gerada é universo.

Com essa informação, se voltarmos 19 posições nos rotores e decriptarmos o ciphertext inteiro, teremos o seguinte plaintext:
```
A RESPOSTA PARA A VIDA, O UNIVERSO E TUDO MAIS É (QUARENTA E DOIS)
```
O texto entre paretenses é a flag Ganesh{QUARENTA E DOIS}.

Coloca a flag, e foi!