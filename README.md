# Álgebra Linear Computacional (UFRRJ-20181)
Um projeto para o acompanhamento das práticas na disciplina de Álgebra Linear Computacional da UFRRJ durante o período 2018/1.

## Clonando o repositório
Como o presente projeto está hospedado no Github, deve ser instalado na máquina o cliente para o protocolo Git, e esse cliente pode ser encontrado nesse [link](https://git-scm.com/downloads) conforme a plataforma da máquina (geralmente o cliente git já vem instalado em algumas distribuições do linux).
Após a instalção do git, este projeto pode ser replicado (clonado) para uma máquina local através dos seguintes comandos:
```shell
cd ~
mkdir git
cd git
git clone https://github.com/fabriciorsf/ufrrj20181-alc.git
cd ufrrj20181-alc
```
O comando acima clona o projeto no diretório `git` criado dentro do diretório padrão do usuário (no Linux é indicado por `~`, no Windows esse caracter deve ser substituído por `%HOMEPATH%`). Alternativamente à linha de comando, outras ferramentas podem ser utilizadas para a sincronização com esse repositório Git: [GitHub Desktop](https://desktop.github.com/), [Sourcetree](https://www.sourcetreeapp.com/) e [TortoiseGit](https://tortoisegit.org/) (outras ferramentas para as diversas plataformas podem ser encontradas [aqui](https://git-scm.com/download/gui)).

Como este projeto é privado, primeiramente é importante que o usuário que pretende clonar tenha acesso ao mesmo (falar com o projessor da disciplina para conceder acesso).

Periodicamente, a réplica local do repositório (i.e, na sua máquina) pode ser sincronizada com o repositório remoto (i.e,., no GitHub) através do seguinte comando:
```shell
cd ~/git/ufrrj20181-alc
git pull --all
```

## Configurações Iniciais
O projeto foi preparado para funcionar com o Python 3.4 ou superior.

### Python e Pip
O Python é uma linguagem de programação, e necessita de um interpretador para que seu código seja executado. O Pip é uma ferramenta para a instalação de bibliotecas (dependências) em python a partir de repositórios remotos (na internet).
Faça o download e instale o [Python](https://www.python.org/downloads/) e [Pip](https://pip.pypa.io/en/stable/installing/). Geralmente o Pip já vem dentro da distribuição do Python, então logo após a instalação do python, teste se o comando `pip` é reconhecido antes de decidir por instalá-lo separadamente.

A documentação de Python pode ser acessada [aqui](https://docs.python.org/), e algumas aulas introdutórias de programação com Python podem ser acessadas [aqui](http://jacarepagua.dcc.ufrj.br/~ladybug/).

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
Com o ambiente ativado, instale essas dependências através do comando abaixo:
```shell
pip install numpy scipy
```
Existem outras questões para se obter uma biblioteca compilada de forma eficiente conforme a arquitetura da máquina. Mas como o propósito desse projeto é apenas didático, tais questões serão desconsideradas. OBS.: se deseja obter o máximo de aproveitamente computacional, considere a instalação de bibliotecas como [Intel MKL](https://software.intel.com/en-us/mkl), [OpenBlas](https://www.openblas.net/), ou [Atlas](http://math-atlas.sourceforge.net/) (considere também a [distribuição de Python da Intel](https://software.intel.com/en-us/distribution-for-python) caso seu processador seja um Intel).

A documentação dessas duas bibliotecas podem ser encontradas nos seguintes links:
* [Scipy](https://www.scipy.org/docs.html)
* [Numpy](https://docs.scipy.org/doc/numpy/)

