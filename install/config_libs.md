## Bibliotecas (Dependências)

Será necessária a instalação de algumas bibliotecas para álgebra linear, a mais conhecida e utilizada atualmente em python é a [Scipy](https://www.scipy.org/), que nada mais é que uma pilha de pacotes/módulos voltados para matemática e engenharias. O módulo mais pertinente a esse projeto chama-se [Numpy](http://www.numpy.org/).

__Com o ambiente virtual ativado__, instale essas dependências através do comando abaixo:
```shell
conda install numpy scipy
```

_Obs.: se está usando o virtualenv, substitua o comando `conda` por `pip`_

Existem outras questões para se obter uma biblioteca compilada de forma eficiente conforme a arquitetura da máquina. Mas como o propósito desse projeto é apenas didático, tais questões serão desconsideradas. OBS.: se deseja obter o máximo de aproveitamente computacional, considere a instalação de bibliotecas como [Intel MKL](https://software.intel.com/en-us/mkl), [OpenBlas](https://www.openblas.net/), ou [Atlas](http://math-atlas.sourceforge.net/) (considere também a [distribuição de Python da Intel](https://software.intel.com/en-us/distribution-for-python) caso seu processador seja um Intel).

A documentação dessas duas bibliotecas podem ser encontradas nos seguintes links:
* [Scipy](https://www.scipy.org/docs.html)
* [Numpy](https://docs.scipy.org/doc/numpy/)


---

[Voltar para __Configurações Iniciais__](./README.md)