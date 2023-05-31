1)QUESTÃO 01: se você passar essa imagem pelo filtro de inversão, qual seria o
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

2)QUESTÃO : faça a depuração e, quando terminar, seu código deve conseguir passar em todos os testes do grupo de teste TestInvertida (incluindo especificamente o que você acabou de criar). Execute seu filtro de inversão na imagem test_images/bluegill.png, salve o resultado como uma imagem PNG e salve a imagem em seu repositório GitHub.

Resposta = usando o comando : python test.py TestInvertida.test_invertida_2
