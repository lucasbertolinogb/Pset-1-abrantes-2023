#1)QUESTÃO 01: se você passar essa imagem pelo filtro de inversão, qual seria o
output esperado? Justifique sua resposta.

• altura: 1

• largura: 4

pixels: [29, 89, 136, 200]

Resposta: seria pixel: [226, 166, 119, 55] , imagine um bastão nele temos um ponto perto de uma 
estremidade e precisamos calcular qual seria a distância para chegar do outro lado e estando na mesma
distância no final do bastão... ou seja , para eu fazer isso eu precisaria saber o tamanho do
bastão , no caso da questão é 255 , e para calcular para que um objeto esteja na mesma distância so que do outro
lado eu precisaria calcular o : tamanho pego - tamanho do bastão = X . Porém , o número seria 
negativo então eu iria inverter o resultado ,
logo me retornando um obejeto do outro lado na mesma distância da extremidade 

2)QUESTÃO 02: faça a depuração e, quando terminar, seu código deve conseguir passar em todos os testes do grupo de teste TestInvertida (incluindo especificamente o que você acabou de criar). Execute seu filtro de inversão na imagem test_images/bluegill.png, salve o resultado como uma imagem PNG e salve a imagem em seu repositório GitHub.

Resposta = usando o comando : python test.py TestInvertida.test_invertida_2

QUESTÃO 03: considere uma etapa de correlacionar uma imagem com o seguinte
kernel:

Na questão é usado um calculo para calcular o valor central: 

Ox,y =Ix−1,y−1 × k0,0 + Ix,y−1 × k1,0 + Ix+1,y−1 × k2,0+ (1)<br>
Ix−1,y × k0,1 + Ix,y × k1,1 + Ix+1,y × k2,1+ (2)<br>
Ix−1,y+1 × k0,2 + Ix,y+1 × k1,2 + Ix+1,y+1 × k2,2 (3)<br>

Nisso eu peguei o pixel da imagem(I) do meio como posição I(1,1) como o centro, e dela fui trocando nos cálculos 
e nessa questão ficou assim:

  Ox,y =80 × k0,0 + 53× k1,0 +  99 × k2,0+(1)<br>
 129× k0,1 +127× k1,1 +148 × k2,1+(2)<br>
 175 × k0,2 + 174 × k1,2 + 193 × k2,2 (3)  <br>
 
Depois disso troquei o kernel proposto na questão do K nas posições indicadas ,resultando nesse cálculo:

  Ox,y =80 × 0 + 53× (-0,07) +  99 ×0+(1)<br>
 129× (-0,45) +127× 1,2 +148 × (-0,25)+(2)<br>
 175 × 0 + 174 × k1,2 + 193 × 0 (3)  <br>
 
E finalmente fiz os cálculos :

   0  +    (-3,71) +   0  +<br>
(-58,05)  +152,4 + (-37) + <br>
     0  +  (-20,88) +   0  <br>
     
Resultando em : 32,76 ou aproxidamente 33 
