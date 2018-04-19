# Instalando o Python com um Ambiente Virtual

O Python é uma linguagem de programação, e necessita de um interpretador para que seu código seja executado. O Pip é uma ferramenta para a instalação de bibliotecas (dependências) em python a partir de repositórios remotos (na internet).

É possível instalar o Python através do download direto do instalador disponível no [site oficial](https://www.python.org/). Mas, como geralmente é necessário a instalação de algumas bibliotecas em python, e para evitar problemas de conflito entre as diversas bibliotecas (dependências) dos projetos em python que possam ser executados em uma mesma máquina, é importante que se trabalhe em um ambiente reservado para o atual projeto (recomenda-se um ambiente para cada projeto independente). Para isso, existem algumas ferramentas de criação desses ambientes, conhecidos como ambientes virtuais. Algumas dessas ferramentas são bastantes conhecidas, como a [Anaconda](https://anaconda.org/anaconda/python), ou a sua versão simplificada e exclusiva para python, a [Miniconda](https://conda.io/miniconda.html), ou mesmo o [Virtualenv](https://virtualenv.pypa.io/en/stable/) que já está incluso na distribuição padrão do python.

Portanto, diante essas possibilidades, a instalação do python com um ambiente virtual pode ser feita através de uma das instruções contidas nos links a seguir, conforme as restrições de acesso à máquina ou preferência pessoal:

* [Python + Pip + Virtualenv](./config_env_virtualenv.md) (necessita do acesso de super-usuário da máquina)
* [Miniconda](./config_env_miniconda.md) (Python e Pip já inclusos, e não necessita do acesso de super-usuário)


---

[Voltar para __Configurações Iniciais__](./README.md)