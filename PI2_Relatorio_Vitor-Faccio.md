# Projeto Integrador 2 - 2019/1

>Instituto Federal de Santa Catarina - *Campus* Florianópolis
>Departamento Acadêmico de Eletrônica
>Curso de Engenharia Eletrônica
>Aluno: 
- Vítor Faccio - <vitorfaccio.ifsc@gmail.com>
>Professores: 
- Fernando Miranda - <fernando.miranda@ifsc.edu.br>
- Luís Azevedo - <azevedo@ifsc.edu.br>

# Introdução
De acordo com o dicionário Michaelis, o termo “revolução” pode ser descrito como uma mudança profunda em algum ambiente ou sistema. Desta forma, conforme Branco (s.d.i.), caracterizam-se respectivamente as três revoluções industriais datadas nos séculos XVIII, XIX e XX: a invenção da máquina a vapor e sua inserção na manufatura têxtil, a aplicação da eletricidade nas indústrias e a integração entre ciência e produção.


As inovações do século XXI estão protagonizando uma quarta revolução industrial e tecnológica, que já é reconhecida globalmente no campo acadêmico e econômico. A “Indústria 4.0”, como pode ser chamado o novo patamar tecnológico, se difere das outras pela convergência entre os mundos físico, digital e biológico no âmbito industrial mas também escapando para o cotidiano das cidades. 


Destaca-se neste ambiente a robótica, o trânsito de dados, a comunicação entre equipamentos e a inteligência artificial. O aprimoramento das indústrias atuais requer a eliminação de ociosidade e disperdícios, o que flerta com o desenvolvimento de máquinas inteligentes. A informatização do chão de fábrica é capaz de tornar todo o processo de fabricação um ciclo controlado e otimizado, abrindo ainda espaço para a comunicação das máquinas com seres humanos e a redução de custos. 


Neste sentido é necessário haver uma boa base de armazenamento remoto de dados, possibilitando assim uma troca de informações rápida e eficiente com os mais diversos aparelhos. O armazenamento em nuvem surge ao lado da inteligência artificial como campo de desenvolvimento para a independência das máquinas na indústria, de forma que não seja mais pertinente uma mão humana controlando e tomando decisões.


A indústria 4.0 já possui relevância mundial: o Fórum Econômico Mundial, evento onde são tratados os rumos das grandes potências empresariais e governamentais do mundo, discute a presença destas inovações tecnológicas no futuro da economia mundial. O Fórum (2016) apresenta uma série de recomendações a líderes industrais para a adequação digital, como a criação de modelos de negócio digitais, digitalização dos planos estratégicos, aproveitamento de dados e integração da automação à força de trabalho. Mais tarde, o Fórum cita (2017) as 10 tecnologias mais emergentes do ano: todas se envolvem com o desenvolvimento de pesquisa e produção, mas três se relacionam especificamente com a eletrônica e a indústria 4.0, como a interação entre equipamentos na lavoura para gerar safras com mais precisão.


# Proposta
Este projeto visa o domínio e a compreensão de técnicas de projeto na engenharia eletrônica, abordando diversos aspectos da criação de um produto. A proposta se dá em torno da linha de produção de uma garrafa de suco de uva, de forma que se obtenha ao fim do semestre um sistema capaz de agir como captador de dados e aplicável em uma indústria real. É tido como foco dos estudos a organização do projeto em quatro níveis:
1. Concepção
    * Definir as necessidades do cliente
    * Considerar tecnologias, estratégias e regulamentações
    * Desenvolver conceitos, técnicas e planos
2. Design
    * Plantas, desenhos e algoritmos que descrevem o que será implementado
3. Implementação
    * Transformação do design em produto
    * Manufatura, escrita de códigos, testes e validações
4. Operação
    * Utilizar o produto implementado para a entrega do serviço definido
    * Manutenção, evolução e recolhimento do sistema


Tendo isso em vista, é dado início à etapa de concepção do projeto.


# Concepção
O estágio de concepção serve como momento para o projetista conhecer o ambiente e os objetivos de seu cliente, bem como pré-requisitos e limitações. Desta forma a primeira tarefa realizada é a definição dos pré-requisitos, que devem ser implantados ou apresentados como soluções ao fim do processo. 


O ambiente industrial deve ser simulado em uma mini-bancada de madeira, onde serão inseridos os componentes do projeto para que se tenha um ambiente semelhante ao de uma fábrica, evitando as mazelas de uma esteira elétrica. Sobre esta plataforma serão implantados blocos para a realização das seguintes tarefas:
1. Verificação de rotulagem
2. Controle de nível de envase
3. Análise de cores de matéria-prima
4. Leitura OCR (*Optical Character Recognition*) de lote e validade
5. Inspeção e testes

A seguir é feita a análise e definição de tecnologias a serem empregadas em cada ponto. As limitações laboratoriais regem as decisões agora tomadas, pois a empregabilidade do produto final depende de disponibilidade e preço dos equipamentos a serem utilizados. As tecnologias empregadas neste projeto serão descritas a seguir. 

## Tecnologias empregadas
Os cinco blocos citados serão desenvolvidos  com  as seguintes tecnologias e equipamentos:
* Controle de nível de envase
	* Sensor ultrassom XXX ligado a Arduino
	* Obtenção de altura do líquido por ultrassom através do bocal da garrafa
	* Criação de escala para relacionar altura e volume
* Análise de cores de matéria-prima
	* Sensor de cor TCS230 ligado a Arduino
* Inspeção e testes
	* Controle de temperatura do produto
	* Sensor infravermelho XXX ligado a Arduino
* Verificação de rotulagem / Leitura OCR de lote e validade
	* *Webcam* ligada a *notebook*
	* Python
	* União dos dois estágios para utilização de apenas uma câmera
	* Seção de verificação de rotulagem
        * Reconhecimento de padrão de imagem
        * OpenCV
	* Seção de leitura OCR de lote e validade
        * Tesseract OCR

As tecnologias envolvidas com a estrutura do projeto, que garantem o funcionamento e a comunicação destes blocos, devem seguir a possibilidade de serem transportadas a uma planta industrial, havendo a substituição de uma plataforma modelo por uma real. Desta forma, elas são definidas como as seguintes:
* Um sensor de presença XXX em cada estágio do processo
* Arduino Uno e *notebook* conectados via serial
* Estrutura física
	* Impressão 3D de alças para a bancada
	* Manufatura de peças em madeira para fixação dos sensores


# Design










