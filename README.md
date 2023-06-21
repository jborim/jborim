### Hi there 👋
Os processos morfológicos são a extração ou modificação de imagem. Neste caso foi usado o google colab e iniciamos o código importando o cv2 para analisar a imagem e o numpy para ajudar executar as matrizes.
Em seguida identificamos onde cada processo de morfologia será usado.
O cv2.imread irá analisar ‘j.png’. 
O img_opening é indicado a variável ‘j_ruidos.png’ para “aumentar” a imagem e limpar os fragmentos de imagem.
O img_closing é indicado a variável ‘j_furos.png’ para “aumentar” a imagem e tapar os furos dentro do j.
Definimos altura e largura em img.shape e o tamanho da matriz, aqui será usada 5x5, na kernel.
Declaramos a erosão e dilatação que é necessária para abertura e fechamento, em iterations=2 é a quantidade de vezes que o efeito vai passar.
Antes de imprimir as imagens, já incorporamos as funções as variáveis e agora a gradiente vai gerar o contorno na primeira imagem, abertura vai usar a erosão seguida da dilatação e o fechamento usa a dilatação em seguida da erosão.
 Por fim, cada imagem é imprimida separado.











