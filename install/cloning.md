# Clonando o repositório (opcional)

*Esta etapa é opicional, uma vez que todo o material pode ser acessado via web diretamente no endereço [https://github.com/fabriciorsf/ufrrj20181-alc/](https://github.com/fabriciorsf/ufrrj20181-alc/). Este passo deve ser executado, apenas se pretende-se manter uma cópia local do repositório.*

Como o presente projeto está hospedado no Github, deve ser instalado na máquina o cliente para o protocolo Git, e esse cliente pode ser encontrado nesse [link](https://git-scm.com/downloads) conforme a plataforma da máquina (geralmente o cliente git já vem instalado em algumas distribuições do Linux).

Se seu sistema for Linux e possuir suporte ao `apt-get`, a instalação é simples e direta através do comando:
```shell
sudo apt-get install git
```

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


---

[Voltar para a página inicial](../README.md)