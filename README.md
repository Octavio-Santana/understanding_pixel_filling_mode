# Entendendo o modo de preenchimento de pixels em transformações de imagens
-----
O método ImageDataGenerator é uma função da biblioteca TensorFlow que permite gerar imagens aumentadas em tempo real durante o treinamento de modelos de aprendizado de máquina. O ImageDataGenerator permite que você defina uma série de transformações para serem aplicadas às imagens durante o treinamento. Isso pode incluir rotações, ampliações, cortes, zoom, inversão horizontal, entre outras opções. Você pode definir essas transformações por meio de parâmetros como `rotation_range`, `width_shift_range`, `height_shift_range`, `zoom_range`, `horizontal_flip`, entre outros.

Além disso, o ImageDataGenerator permite escolher um `fill_mode` para preencher as áreas vazias resultantes da rotação ou outras transformações. Existem quatro opções disponíveis:

* constant: preenche com um valor constante especificado pelo parâmetro `cval`;
* nearest: preenche com o valor do pixel mais próximo;
* reflect: reflete a imagem em relação à borda da imagem;
* wrap: envolve a imagem para preencher as áreas vazias;