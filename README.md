# desafio_stepps
Código de implementação do desafio técnico da empresa Stepps

O objetivo do desafio é:
1. Fazer uma CONTAGEM da quantidade de mamões presentes na imagem
2. Diante do vídeo disponibilizado no arquivo “Teste_Video.MP4”, quantos mamões ultrapassam a linha amarela, considerando o período de tempo entre 00:05 segundos e 00:35 segundos.

# Implementação
Para implementação desse desafio, foi utilizada técnicas de PDI e deep learning, em especial segmentação por limiarizações e por, em especial, com o formato HSV da imagem, além de utilizar a segmentação por _watershed_, que é uma técnica bem conhecida para quando se tem objetos encostando um no outro ou sobrepostos, pois ela trata a imagem como se fosse um mapa topográfico. 

As técnicas de segmentação foram utilizadas para a primeira etapa do desafio, para a contagem da quantidade de mamões presentes na imagem, tendo um resultado um pouco melhor a segmentação por cores.

Para a contagem de mamões que passam da linha amarela do vídeo foi utilizada a yolov11, treinado um modelo com a base de dados fornecida pela empresa, e realizada a contagem mostrada automaticamente em vídeo.

O vídeo final com a contagem está intitulado e está no link : [object_counting_output.mp4](https://drive.google.com/drive/folders/1dYmUsJFKakl67yf946pqs-jvp42bPHJd?usp=sharing) 

O print da contagem dos mamões do teste 1: [mamoes_contagem_1](https://drive.google.com/file/d/1EJ3MlN0o_7Ja2Wn0bmwRoTQdhQCeFMNr/view?usp=drive_link)

Por conta de limitação, o dataset com as imagens e labels de treinamento e também os vídeos, que foi fornecido pela empresa, naõ foi colocado no git, até por uma questão mais ética também, e por isso, caso necessário realizar o treinamento do modelo, images e labels devem ficar na pasta dataset junto com o .yaml

Para o Teste_Video.mp4, ele deve ser colocado em uma pasta chamada video/Teste_Video.mp4

