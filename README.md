## Descrição

Este repositório contém um aplicativo que converte uma imagem em uma canção. O aplicativo foi escrito em Python e utiliza a biblioteca Streamlit para criar uma interface de usuário web interativa. Este projeto é uma adaptação do trabalho original de [Victor Murcia](https://github.com/victormurcia). Victor tem trabalhos muito interessantes na intersecção de música, arte e programação.

O código é composto por várias funções que implementam a geração de notas musicais e a criação de uma escala musical a partir das imagens fornecidas. A imagem é convertida em uma canção utilizando a análise de cor de seus pixels, que são mapeados para diferentes notas musicais.

## Como usar

Este aplicativo é baseado na web e pode ser executado localmente usando o Streamlit. Para isso, instale as dependências necessárias listadas no arquivo `requirements.txt` e execute o comando `streamlit run <nome do arquivo.py>`.

Na interface do usuário, você pode carregar sua própria imagem ou selecionar uma imagem de exemplo. Em seguida, você pode escolher a escala, a tonalidade, a oitava e a harmonia que deseja aplicar à imagem. A imagem carregada será convertida em uma canção baseada nas opções selecionadas. Você também tem a opção de usar pixels aleatórios da imagem e definir a duração de cada nota na canção.

## Dependências

O aplicativo requer as seguintes bibliotecas Python:

- streamlit
- pandas
- numpy
- opencv-python
- Pedalboard
- PIL
- scipy
- librosa
- glob

## Funcionalidades do Código

O código possui várias funções para implementar a geração de música a partir de imagens. As principais funções incluem:

- `get_piano_notes`: Gera as frequências das notas musicais.
- `makeScale`: Cria uma escala musical com base na tonalidade e na oitava selecionadas.
- `hue2freq`: Converte um valor de tonalidade (hue) em uma frequência musical.
- `img2music`: Converte uma imagem em uma canção.