# Aula 6 - Criar e config a VM, Logar o linux, install o ssh no vscode e fazer o Hello Word no Nasm!

### ☆ Configurações do sistema VM Fedora:

★ Dois nucleos de processador: 

![f3.PNG](https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/8ed0aa37-58f1-4532-990e-ba7df09a6ac6/f3.png)

★ Memoria: 4096:

![fedora2.PNG](https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/a944291c-6e14-4ad3-abe4-96a083580aaa/fedora2.png)

★ Monitor: 128 MB:

![f4.PNG](https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/30156edc-b90c-42e3-aa00-24df7e54aff7/f4.png)

★ REDES: 

↳ Avançado → Redirecionamente de Portas 

(https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/9afc7d30-264b-42e7-b1e4-b0dce435d220/f6.png)

**𓇼Pode deixar em modo NAT**

----
★ Fazendo a conexão cocpitk 

    ✦ FEDORA | PROT TCP | 127.0.0.1 | 9090 | 10.0.2.15 | 9090

![f7.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/a7b35610-a34d-4bcc-a309-bc9a11e713db/f7.png)

---

*✦ Em armazenamento, criar um vhd* 

![f5.PNG](https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/9d79da49-6cc6-460a-9f04-c5f98856d644/f5.png)

---

---

☆ ***Config do linux ja feita!!***

![local.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/52da7839-1992-407c-aef5-325141e0e08e/local.png)

---

---

127.0.0.1 = [LocalHost/LoopBack](https://www.youtube.com/watch?v=PxefrYrDYWk)

    localhost; nome dado ao local/maquina que esta trabalhando sua conexão.
    127.0.0.1 - é necesario para manter a segurança e comodide (app não precisa acessar a internet para fazer alguma conexão interna com a maquina). 
    Em outras palavras, indica que o servidor esta no mesmo local que a conexão 
 

### ☆ Acessando a maquina virtural pelo endereço loopback

    ★ acessar o link no navegador ↠ https 127.0.0.1:9090

    ★ acessar minha conta de usuario do linux

![f7.PNG](https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/0701bb09-614d-477f-9af5-d2a44fc28667/f7.png)

----
### ☆ Fazendo as instalações iniciais do linux 

    ★ sudo dnf update && upgrade 

- **DNF:** é um gerenciador de pacotes para sistemas operacionais que utilizam pacotes RPM
- **UPDATE**: é usado para ***baixar as atualizações*** e informações dos pacotes de todas as fontes (repositórios) configurados.
- **UPGRADE**: é usado para ***instalar as atualizações*** disponíveis dos pacotes instalados atualmente no sistema
- &&: (ENCADIAR) é um operador lógico que ***significa E (and)***. Ele é usado para criar **uma expressão logica** onde o **segundo elemento somente é executado se o primeiro for VERDADEIRO**.
---
***★ Inserir a senha posta no linux: P@$$w0rd***

foto


*(Usando o comando sudo dnf update && sudo dnf upgrade **-y** = *retira as perguntas de confirmação de instalação*)*

***

### ☆ ***comando: uname -a*** *(usado neste caso para verificar a versão do linux)*

    ★ uname = O comando uname, que significa Unix Name, vai mostrar informações detalhadas sobre seu sistema Linux

        ✦ -a = exibe todas as informações do sistema

        ✦ -s = exibe o nome do kernel. 

        ✦ -n = exibe o hostname do node do sistema 

---

★ @@@ --version (conferir se os apt estão install)

    ✦ git

    ✦ nasm 

    ✦ gcc 

    ✦ phyton3 (este esta)
    
---

### ☆  Instalar o git e o nasm

    ✦ sudo dnf install git

    ✦ sudo dnf isntall nasm

**(colocar a senha em ambas installs: P@$$word)** 

![f9.PNG](https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/a8b985ea-f165-4ed0-a6f6-9a8d433907c7/f9.png)

---
### ☆ Após a instalação do git, criar o diretório e inita-lo

    ★ mkdir ProjetoNasm

    ★ cd ProjetoNasm

    ★ git init 

(https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/ea8a63a4-2b53-450f-9045-5095e837e3fc/f10.png)

*não esquecer as config iniciais do git: git config --global user.@@@*

---

---

### ☆ Configurar o SSH no VSCode  

    ★ Redirecionar a porta para SSH

![a.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/4f3219a5-a568-4bc0-8495-6e6d7abac01f/a.png)

    Instalar a extensão do SSH no VS

![a.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/222e6a8d-5605-4356-8199-61a0642ce8f7/a.png)

    ★ Iniciando as configurações da extensão, definimos o locar do arquivo de configuração

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/1b25ccac-2bdd-4c9a-9c3b-58a0a18379c6/Untitled.png)

    ★ Criamos as pastas e um arquivo de texto sem extensão com o nome “config”

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/0e49694f-40aa-4d97-9f08-8fc4d57103f3/Untitled.png)

    ★ Inserimos o comando para conectarmos ao ssh

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/3ae74bd6-c867-43fd-9731-66872402b863/Untitled.png)

    ★ Conectamos e inserimos a senha

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/b38233fa-0ddf-4b32-be15-98dbce0f422a/Untitled.png)

    ★ Apetamos Crtl+L para abrir o terminal

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/80446f4e-5de6-430b-bb10-f6adabe1029e/Untitled.png)

---

---

### ☆ *Criando um arquivo Nasm 

    ★ Add a extensão de icon pra auxiliar 

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/dac7e552-ddc4-4f16-90a3-08c20b9c487c/Untitled.png)

    ★ Criando o arquivo 

    ★ Comitando 

        ↳ *git commit -m “Criação de arquivo”

![vs1 (1).PNG](https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/db23c094-57f8-4f61-8bc6-a3eefba93045/vs1_(1).png)

#### ☆ Codando o arquivo 

    ★ comita-lo novamente 

![vs2 (1).PNG](https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/15f96f34-4abd-483c-9be8-174c9462d2c4/vs2_(1).png)

#### ☆ Com o comando 

    ↳ nasm -f elf hello.asm criamos o seu binario

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/7d28e8c8-4435-4171-92db-2b42cc774223/Untitled.png)

---
![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/97b1b01e-f1a5-44b7-8daf-a69bc364ee86/Untitled.png)

    ld - link dynamic (comando do linux)
    Comando Linux ld. Nos sistemas operacionais do tipo Unix, o ld **é um vinculador**. Ele combina vários objetos compilados e arquivos compactados, realoca seus dados e vincula referências de símbolos. Normalmente, o último passo na compilação de um programa é executar o ld 
 
    -m → make
    elf_i386 → arquitetura. (i386 → 32Bits i64 → 64 bits)
    -o →Objeto.  (nome do arquivo)
 
    No total temos o arquivo hello, o binario desse arquivo “hello.o” e com o ld criamos um executavel com esses arquivos
 

![vs3 (2).PNG](https://prod-files-secure.s3.us-west-2.amazonaws.com/6910beb1-da0c-4082-91cb-9d9570c1f042/edeb870c-1433-4cd0-ae0a-5af74527721d/vs3_(2).png)

☆ Encaminhar para o git

foto

>git push -u oringin main é utilizado quando queremos enviar a branch que criamos para o repositório remoto. Isso criará um “elo” entre o seu repositório local e o repositório remoto. 