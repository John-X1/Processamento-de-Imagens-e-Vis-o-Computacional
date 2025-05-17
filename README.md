# Projeto de Reconhecimento de Imagem em Tempo Real com Webcam
     
Este projeto implementa um sistema de reconhecimento de imagem em tempo real, utilizando um modelo de aprendizado de máquina previamente treinado através da plataforma Teachable Machine. O software captura o fluxo de vídeo da câmera do computador, analisa cada quadro individualmente para identificar a presença de objetos ou categorias de imagens que foram ensinadas ao modelo durante o treinamento. O resultado dessa análise, que consiste na classe prevista para o que está sendo visualizado e o nível de confiança dessa previsão, é então sobreposto diretamente na tela, proporcionando um feedback visual imediato.

Possíveis Aplicações: Identificação básica de objetos, controles simples baseados em visão (com adaptações), projetos educacionais e de aprendizado e auxílio visual fundamental em contextos específicos.

# Instruções de Instalação:
Arquivos Necessários: keras.model.h5 (modelo treinado) e labels.txt (lista de rótulos).

Geração dos Arquivos (Teachable Machine): Exporte o modelo treinado como "TensorFlow Lite" e selecione "Keras (.h5)". Baixe também o arquivo labels.txt.

Local de Salvamento dos Arquivos: Salve keras.model.h5 e labels.txt na mesma pasta do script Python.


# Instruções de Uso:

Pré-requisitos de Software: Python instalado e as bibliotecas tensorflow, opencv-python, e numpy instaladas via pip install tensorflow opencv-python numpy.

Execução do Código: Salve o código Python como .py, certifique-se de que os arquivos do modelo e rótulos estão na mesma pasta, e execute via terminal com python nome_do_arquivo.py.

Utilização da Câmera: O código usa cv2 para acessar a câmera padrão (índice 0). Uma janela "Imagem da Webcam" exibirá o feed com as previsões.

Seleção de Diferentes Câmeras: Modifique a linha camera = cv2.VideoCapture(0) para outros índices inteiros (1, 2, etc.) para tentar acessar outras câmeras conectadas. A numeração pode variar dependendo do sistema. Feche outros aplicativos de câmera se houver problemas.

Encerramento do Programa: Pressione a tecla ESC enquanto a janela "Imagem da Webcam" estiver em foco para fechar o programa e liberar a câmera.


# Creditos:
O trabalho foi realizado no Laboratório de Sistemas de Informação(LABSI 01) da UFOPA-CORI.
