---
title: A Melhor Criação da Microsoft
---
[← Voltar ao blog](https://blog.pedromclaro.com)
<p class="post-info"><strong>2 min de leitura</strong> • <i class="tag1__linux">linux</i> <i class="tag2__microsoft">microsoft</i> <i class="tag3__tutorial">tutorial</i></p>


## A melhor Criação da Microsoft
> ### "Se a Microsoft já ama o Linux, então eu já ganhei" - Linus Torvalds

É meus amigos, faz um bom tempo que a Microsoft passou a adotar e apoiar o Linux em seus produtos e serviços.

Hoje vamos explorar um pouco da maravilha que é o **Windows Subsystem for Linux.**

Bom basicamente o WSL é uma ferramenta que nos permite rodar o Linux dentro do Windows.

### Como exatamente o WSL funciona?

Assim como existem softwares como o **Oracle Virtual Box** que nos permite instalar outros sistemas operacionais em nossa máquina, o funcionamento do WSL é parecido, mas "a grosso modo" foi feito para gastar menos recursos se comparado a instalarmos distros Linux dentro do Virtual Box.

### Instalando o WSL

Primeiro, abra seu Windows Terminal no modo administrador.

A instalação é bem simples, basta digitar: `wsl --install`

Com este comando já vamos instalar o ambiente Linux e também o Ubuntu.

Após a conclusão da instalação, será necessário reiniciarmos o computador. Ao ligar novamente, uma janela do Windows Terminal será aberta para continuarmos configurando nosso ambiente Linux.

### Configurando o ambiente Linux

Com a janela do terminal aberta, configure seu nome de usuário e sua senha. Assim como em qualquer distro, a senha será utilizada para realizarmos tarefas administrativas.

Pronto, agora o Ubuntu está disponível para uso assim como em um servidor ou no Virtual Box.
___

É interessante que existe uma integração entre o file sistem do Windows e o file sistem do Linux instalado.
Você facilmente pode acessar os arquivos do Ubuntu pelo explorador de arquivos como se fosse uma pasta compartilhada em rede:

![](https://i.ibb.co/n3Mj05X/wsl.gif)

### Instalação de Distros no WSL 2

Podemos gerenciar o WSL 2 diferentemente do WSL 1. Isso nos dá a possibilidade de instalarmos outras distribuições!

No seu terminal digite: `wsl -l -o`

Veremos uma lista das distribuições disponíveis de forma oficial (sim a comunidade já deu um jeito de rodar outras distribuições, como o ArchLinux por exemplo.)

Dentre elas temos o Debian, kali Linux, openSUSE...

Para fazer a instalação de alguma, digite: `wsl --install <nome da distro>`

Irei instalar o Kali Linux como exemplo.

Será necessário assim como no Ubuntu, configurarmos nosso nome de usuário e senha. Após a instalação, podemos alternar de distribuição de uma forma bem fácil pelo Windows Terminal:

![](https://i.ibb.co/N3J8B2S/wsl-kali.gif)

Se digitarmos no terminal: ` wsl --list --verbose`

Veremos as distros instaladas, quais estão rodando nesse momento, qual está parada e suas versões.

Você verá que no Ubuntu, ao seu lado tem um asterisco, o que significa que ele é a nossa distro principal, nossa distro padrão. Podemos mudar com o comando: `wsl --set-default <nome da distro>`

Para remover uma distro Linux do WSL digite o seguinte comando: `wsl --unregister <nome da distro>`

E claro, você pode digitar: `wsl --help` Para ver outros comandos importantes.

Enfim, podemos instalar Docker e por ele instalar outros programas e outras distribuições, até aplicativos com interface gráfica dá pra rodar com o WSL.

O Linux é muito versátil, podemos usá-lo desde em [uma batata](https://www.bbspot.com/news/2008/12/linux-on-a-potato.html) até no Windows :)

---

Escrito por [@pedromclaro](https://www.pedromclaro.com)

[← Voltar ao blog](https://blog.pedromclaro.com)