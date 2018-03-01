Contador de Ciclistas
=====================

Projeto experimental de contagem de ciclistas utilizando webcam de baixo custo.
Quer implantar contadores digitais de ciclistas na cidade de Curitiba?

A Cicloiguaçu está chamando programadores, estudantes, startups e hackers para implantar o primeiro contador digital de ciclistas da cidade de Curitiba, e você pode fazer parte do time!

![Contador em Curitiba](http://www.cicloiguacu.org.br/wp-content/uploads/2016/08/09.png)


------------------------

**O que precisamos no momento:**
* Mais vídeos para testes!
* Entender o código dos arquivos para configurar de acordo com cada locação:
- Parâmetros no .camera.conf
- CycloTracker.cpp
Inicialização da câmera à partir da linha 275

**[Confira as issues](https://github.com/cicloiguacu/ContadorDeCiclistas/issues) e as [atividades do projeto](https://github.com/cicloiguacu/ContadorDeCiclistas/projects/1)**
------------------------

Por volta de 2 anos atrás o LabProdam, Laboratório de Inovação da Prefeitura de São Paulo lançou um projeto experimental de contagem de ciclistas utilizando webcam de baixo custo. Este projeto teve um grande sucesso devido à considerável precisão na contagem dos ciclistas.

![Contador LabProdam](http://www.cicloiguacu.org.br/wp-content/uploads/2017/01/ciclistas-contador-700x528.jpg)

[Clique no link para ver um vídeo sobre o projeto](https://www.youtube.com/watch?v=x8cXPX41zuM)

Queremos implantar um sistema semelhante em Curitiba para contribuir nas políticas públicas de ciclomobilidade. Uma versão no Github da Cicloiguaçu já está disponível e seu código-fonte em C++ foi disponibilizado para qualquer um ajudar no projeto.
https://github.com/cicloiguacu/ContadorDeCiclistas


O trabalho é colaborativo e voluntário, mas a Cicloiguaçu pode emitir um certificado de trabalho neste projeto, caso você queira.


Quer ajudar? Entre em Contato conosco!

Pelo site: www.cicloiguacu.org.br

Pelo Facebook – https://www.facebook.com/Cicloiguacu/

Por e-mail – projetos@cicloiguacu.org.br

Atividades a serem desempenhadas:

* Implantação de um protótipo de Sistema de contagem
* Levantamento de equipamentos
* Identificação de locais para testes
* Geração de vídeos para teste
* Visitas in loco
* Programação
* Validações
* Avaliação dos resultados obtidos
* Aplicação de um sistema definitivo
* Projetar expansão do sistema
* Estudar novas possibilidades de sistemas
* Melhorar precisão através de Inteligência Artificial e múltiplas câmeras
* Aplicar novas tecnologias de detecção de objetos como o [YOLO: Real-Time Object Detection](http://pjreddie.com/darknet/yolo/) ![Teste YOLO com imagem](http://www.cicloiguacu.org.br/wp-content/uploads/2017/01/predictions01.jpg) ![Teste 2](http://www.cicloiguacu.org.br/wp-content/uploads/2017/01/predictions02.jpg)
* Identificar como a solução auxilia no desenvolvimento das contagens tradicionais. [Exemplo de trabalho PDF](http://multimidia.curitiba.pr.gov.br/2015/00159285.pdf) [Exemplo](http://www.cicloiguacu.org.br/wp-content/uploads/2016/08/contador-ciclistas-20170126.png)

Não possui os requisitos? Você pode ajudar ajudando a divulgar esta chamada! Se quiser ajudar ainda mais, entre em contato conosco mesmo assim 😉 Sempre há muito o que fazer na Cicloiguaçu!

O [Carlos Delfino](http://carlosdelfino.eti.br/ContadorDeCiclistas/) andou fazendo um trabalho sensacional:

> Este é um fork do projeto original para contagem de ciclistas em ciclovias e ciclofaixas. O objetivo do fork é contribuir principalmente com o projeto original gerando um Port para RaspeberryPI e para NanoPI em principal.

(GitHub)[https://github.com/carlosdelfino/ContadorDeCiclistas]

-----------

Requisitos
-----------

- OpenCv 2.4
- V4l2Loopback
- WebCam

Como Usar
---------

- Compilar a aplicação digitando na linha de comando:
make

- Iniciar a aplicação utilizando a linha de comando abaixo:

`bin/CycloTracker usage:`

	--help   (-h): print this message. 
	--override (-O): override point picked parameters.
	--reg_source (-s) <file_name>: Specify regular file where data comes from.
	--dev_source (-D) <number>: Specify device number where data comes from.
	--record (-r) <file_name>: Record video to filename.
	--stream (-S) <device>: Streams video via device.
	--sensor (-t) <device>: Specify device file which is a sensor.
	--address (-a) <address>: address must be present and must be in in this format: street-number. --address faria_lima-1200.

Exemplo:

`bin/CycloTracker -D 0 --address Faria_Lima-2152 --record out.avi -S /dev/video1`

- Necessário selecionar (clicando na tela com o endereço fornecido):

1) O ponto em que o contador amarelo de ciclistas da direita para a esquerda deve se localizar
2) O ponto em que o contador amarelo de ciclistas da esquerda para a direita deve se localizar
3) O ponto superior esquerdo da área em perspectiva 
4) O ponto superior direito da área em perspectiva
5) O ponto inferior esquerdo da área em perspectiva
6) O ponto inferior direito da área em perspectiva
7) O ponto superior esquerdo da área de corte (vermelha)
8) O ponto inferior direito da área de corte (vermelha)
