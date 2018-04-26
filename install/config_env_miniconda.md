# Miniconda

O [Miniconda](https://conda.io/miniconda.html) é uma ferramenta para facilitar a criação e configuração de ambientes virtuais em Python. E é um subprojeto do [Conda](https://conda.io/), um projeto maior para ambientes virtuais.

## Download e Instalação

Faça o Download e Instalação do Miniconda com um dos comandos abaixo, conforme seu sistema operacional.


* [Linux 64-bit](https://conda.io/docs/user-guide/install/linux.html)

```shell
wget https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda.sh
bash ~/miniconda.sh -b -p $HOME/miniconda
export PATH="$HOME/miniconda/bin:$PATH"
```


* [Linux 32-bit](https://conda.io/docs/user-guide/install/linux.html)

```shell
wget https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86.sh -O ~/miniconda.sh
bash ~/miniconda.sh -b -p $HOME/miniconda
export PATH="$HOME/miniconda/bin:$PATH"
```


* [MacOS](https://conda.io/docs/user-guide/install/macos.html)

```shell
wget https://repo.continuum.io/miniconda/Miniconda3-latest-MacOSX-x86_64.sh -O ~/miniconda.sh
bash ~/miniconda.sh -b -p $HOME/miniconda
export PATH="$HOME/miniconda/bin:$PATH"
```


* [Windows 64-bit](https://conda.io/docs/user-guide/install/windows.html) - Primeiramente faça o [download](https://repo.continuum.io/miniconda/Miniconda3-latest-Windows-x86_64.exe), e depois execute o comando:

```shell
start /wait "" Miniconda4-latest-Windows-x86_64.exe /InstallationType=JustMe /RegisterPython=0 /S /D=%UserProfile%\Miniconda3
```


* [Windows 32-bit](https://conda.io/docs/user-guide/install/windows.html) - Primeiramente faça o [download](https://repo.continuum.io/miniconda/Miniconda3-latest-Windows-x86.exe), e depois execute o comando:

```shell
start /wait "" Miniconda4-latest-Windows-x86.exe /InstallationType=JustMe /RegisterPython=0 /S /D=%UserProfile%\Miniconda3
```


### Criação do ambiente virtual

Agora é necessário criar o ambiente virtual que deverá se usado na execução de qualquer código desse projeto. Ao criar o ambiente, o mesmo deve ser identificado por um nome, que será `ufrrj`, conforme o comando abaixo:
```shell
conda update conda
conda create -n ufrrj python=3
```

Se o comando `conda` não for reconhecido, troque `conda` por `~/miniconda/bin/conda`.


### Ativação do ambiente virtual

O próximo passo é a ativação desse ambiente reservado que foi criado no passo anterior. Use o seguinte comando para ativá-lo:
```shell
conda activate ufrrj
```

Dependendo de como foi instalado o `conda`, talvez o comando acima não funcione. Nesse caso, use o comando abaixo, substituindo a variável `$CONDA` pelo camiho de instalação dos arquivos binários do `conda`.
```shell
source $CONDA/activate ufrrj
```

Obs.: O diretório padrão de instalação do miniconda no linux é o seguinte caminho `~/miniconda`, portanto os binários estão nesse caminho `~/miniconda/bin`. , caso o cominho de instalação seja o padrão, o comando correto será o seguinte:
```shell
source ~/miniconda/bin/activate ufrrj
```

### Entrando e Saindo do interpretador python

Com o ambiente previamente ativado, para entrar no interpretador python, execute o comando:
```shell
python
```

E para sair do interpretador python, execute o comando:
```shell
exit()
```

### Desativação do ambiente virtual

Use o seguinte comando para desativar o ambiente virtual:
```shell
conda deactivate
```


---

[Voltar para __Instalando o Python com um Ambiente Virtual__](./config_env.md)