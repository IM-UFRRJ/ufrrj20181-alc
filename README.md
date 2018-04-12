# Álgebra Linear Computacional (UFRRJ-20181)
Um projeto para o acompanhamento das práticas na disciplina de Álgebra Linear Computacional da UFRRJ durante o período 2018/1.

## Clonando o repositório
Este projeto pode ser replicado (clonado) para uma máquina local através dos seguinte comandos:
```shell
cd ~
mkdir git
cd git
git clone https://github.com/fabriciorsf/ufrrj20181-alc.git
cd ufrrj20181-alc
```
O comando acima clona o projeto no diretório `git` criado dentro do diretório padrão do usuário (no Linux é indicado por `~`, no Windows esse caracter deve ser substituído por %HOMEPATH%).
Como este projeto é privado, primeiramente é importante que o usuário que pretende clonar tenha acesso ao mesmo (falar com o projessor da disciplina para conceder acesso).

## Configurações Iniciais
O projeto foi preparado para funcionar com o Python 3.4 ou superior.

### Python e Pip
O Python é uma linguagem de programação, e necessita de um interpretador para que seu código seja executado. O Pip é uma ferramenta para a instalação de bibliotecas (dependências) em python a partir de repositórios remotos (na internet).
Faça o download e instale o [Python](https://www.python.org/downloads/) e [Pip](https://pip.pypa.io/en/stable/installing/). Geralmente o Pip já vem dentro da distribuição do Python, então logo após a instalação do python, teste se o comando `pip` é reconhecido antes de decidir por instalá-lo separadamente.

### Ambiente Virtual
Como é necessário a instalação de algumas bibliotecas, e para evitar problemas de conflito entre as diversas bibliotecas (dependências) dos projetos em python que possam ser executados em uma mesma máquina, é importante que se trabalhe em um ambiente reservado para o atual projeto (recomenda-se um ambiente para cada projeto independente).
Para isso, existem algumas ferramentas de criação desses ambientes, conhecidos como ambientes virtuais.
Algumas dessas ferramentas são bastantes conhecidas, como a [Anaconda](https://anaconda.org/anaconda/python), ou a sua versão simplificada e exclusiva para python, a [Miniconda](https://conda.io/miniconda.html).
Este tutorial irá instruir sobre o uso da ferramenta que já está inclusa na distribuição padrão do python, conhecida como [Virtualenv](https://virtualenv.pypa.io/en/stable/), e pode ser instalada através do seguinte comando:
```shell
pip3 install virtualenv
```
Agora é necessário criar o ambiente virtual que deverá se usado na execução de qualquer código desse projeto. Ao criar o ambiente, o mesmo deve ser identificado por um nome, que será `ufrrj`, conforme o comando abaixo:
```shell
cd ~/git/ufrrj20181-alc
virtualenv ufrrj
```
Perceba que foi criado um diretório com o nome do ambiente (dentro do diretório em que foi executado o comando acima: `~/git/ufrrj20181-alc`). O próximo passo é a ativação desse ambiente reservado que foi criado no passo anterior. Use o seguinte comando para ativá-lo:
```shell
source ufrrj/bin/activate
```

### Bibliotecas (Dependências)
Será necessária a instalação de algumas bibliotecas para álgebra linear, a mais conhecida e utilizada atualmente em python é a [Scipy](https://www.scipy.org/), que nada mais é que uma pilha de pacotes/módulos voltados para matemática e engenharias. O módulo mais pertinente a esse projeto chama-se [Numpy](http://www.numpy.org/).
Instale essas dependências através do comando abaixo:
```shell
pip install numpy scipy
```
Existem outras questões para se obter uma biblioteca compilada de forma eficiente conforme a arquitetura da máquina. Mas como o propósito desse projeto é apenas didático, tais questões serão desconsideradas. OBS.: se deseja obter o máximo de aproveitamente computacional, considere a instalação de bibliotecas como [Intel MKL](https://software.intel.com/en-us/mkl), [OpenBlas](https://www.openblas.net/), ou [Atlas](http://math-atlas.sourceforge.net/) (considere também a [distribuição de Python da Intel](https://software.intel.com/en-us/distribution-for-python) caso seu processador seja um Intel).
