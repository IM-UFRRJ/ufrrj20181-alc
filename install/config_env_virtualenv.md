# Python + Pip + Virtualenv

As instruções a seguir necessitam do acesso de super-usuário da máquina. Se não possui tal nível de acesso, recomenda-se usar o python a partir da instalação do Miniconda, cujas instruções estão contidas nesse [link](./config_env_miniconda.md). 

## Python e Pip
Faça o download e instale o [Python](https://www.python.org/downloads/) e [Pip](https://pip.pypa.io/en/stable/installing/). Geralmente o Pip já vem dentro da distribuição do Python, então logo após a instalação do python, teste se o comando `pip` é reconhecido antes de decidir por instalá-lo separadamente.

Se seu sistema for Linux e possuir suporte ao `apt-get`, a instalação deve ser feita através do comando:
```shell
sudo apt-get install python3 pip3
```

## Virtualenv
O [Virtualenv](https://virtualenv.pypa.io/en/stable/) é uma ferramenta para a criação de ambientes virtuais já está inclusa na distribuição padrão do python, e deve ser instalada através do seguinte comando:

```shell
sudo pip3 install virtualenv
```

Se seu sistema for Windows, remova do comando comando acima o termo `sudo`, e talvez seja necessário executar o comando a partir de um _command prompt_ com permissão de administrador.


### Criação do ambiente virtual

Agora é necessário criar o ambiente virtual que deverá se usado na execução de qualquer código desse projeto. Ao criar o ambiente, o mesmo deve ser identificado por um nome, que será `ufrrj`, conforme o comando abaixo:
```shell
cd ~/git/ufrrj20181-alc
virtualenv ufrrj
```
Perceba que foi criado um diretório com o nome do ambiente (dentro do diretório em que foi executado o comando acima: `~/git/ufrrj20181-alc`).


### Ativação do ambiente virtual

O próximo passo é a ativação desse ambiente reservado que foi criado no passo anterior. Use o seguinte comando para ativá-lo:
```shell
source ~/git/ufrrj20181-alc/ufrrj/bin/activate
```

### Desativação do ambiente virtual

Use o seguinte comando para desativar o ambiente virtual:
```shell
source ~/git/ufrrj20181-alc/ufrrj/bin/deactivate
```


---

[Voltar para __Instalando o Python com um Ambiente Virtual__](./config_env.md)