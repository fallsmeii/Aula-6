# Aula 6 - Criar e config a VM, Logar o linux, install o ssh no vscode e fazer o Hello Word no Nasm!

### ☆ Configurações do sistema VM Fedora:

★ Dois nucleos de processador: 


<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/ddf2027f-47d8-4c6a-b3af-4682eae298cf" width="500px"/>   
</div>


---
★ Memoria: 4096:


<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/ef6561fd-e36e-4353-9e91-a0026f672c66" width="500px" />   
</div>

---
★ Monitor: 128 MB:


<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/05b3be24-9194-454a-a92b-971b9c437c81" width="500px" />   
</div>


---
★ REDES: 

↳ Avançado → Redirecionamente de Portas 

<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/90a26557-23d1-4900-8f14-2943e08a17c8" width="500px" />   
</div>
𓇼 Pode deixar em modo NAT

----
★ Fazendo a conexão cocpitk 

    ✦ FEDORA | PROT TCP | 127.0.0.1 | 9090 | 10.0.2.15 | 9090

<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/b9f3eab2-9bdb-4309-b953-ac9830cf7998" width="500px" />   
</div>

---

*✦ Em armazenamento, criar um vhd* 

<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/e5998200-94cd-42b9-81a8-770eb17f9757" width="500px" />   
</div>

---

---

☆ ***Config do linux ja feita!!***

<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/eee9049e-7856-4463-819c-8d8aafaff756" width="500px" />   
</div>

---

---

>127.0.0.1 = [LocalHost/LoopBack](https://www.youtube.com/watch?v=PxefrYrDYWk)

    localhost; nome dado ao local/maquina que esta trabalhando sua conexão.
    127.0.0.1 - é necesario para manter a segurança e comodide (app não precisa acessar a internet para fazer alguma conexão interna com a maquina). 
    Em outras palavras, indica que o servidor esta no mesmo local que a conexão 
 

### ☆ Acessando a maquina virtural pelo endereço loopback

    ★ acessar o link no navegador ↠ https 127.0.0.1:9090

    ★ acessar minha conta de usuario do linux

<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/2f74e140-2fc2-40a2-b19d-b7c11122d8fc)" width="500px" />   
</div>


### ☆ Fazendo as instalações iniciais do linux 

    ★ sudo dnf update && upgrade 

- **DNF:** é um gerenciador de pacotes para sistemas operacionais que utilizam pacotes RPM
- **UPDATE**: é usado para ***baixar as atualizações*** e informações dos pacotes de todas as fontes (repositórios) configurados.
- **UPGRADE**: é usado para ***instalar as atualizações*** disponíveis dos pacotes instalados atualmente no sistema
- &&: (ENCADIAR) é um operador lógico que ***significa E (and)***. Ele é usado para criar **uma expressão logica** onde o **segundo elemento somente é executado se o primeiro for VERDADEIRO**.

    ★ Inserir a senha posta no linux: P@$$w0rd 

<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/446d8ac1-f1ab-4708-93e0-9b296bb24d2c" width="500px" />   
</div>

*(Usando o comando sudo dnf update && sudo dnf upgrade **-y** = *retira as perguntas de confirmação de instalação*)*

***

### ☆ ***comando: uname -a*** *(usado neste caso para verificar a versão do linux)*

<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/1c2b9203-5620-4916-bd6a-39d6ac5ce19e" width="500px" />   
</div>

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

<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/ff66762d-e4af-45e3-983e-73c5ba7caff8" width="500px" />   
</div>

---
### ☆ Após a instalação do git, criar o diretório e inita-lo

    ★ mkdir ProjetoNasm

    ★ cd ProjetoNasm

    ★ git init 


*não esquecer as config iniciais do git: git config --global user.@@@*

---

---

### ☆ Configurar o SSH no VSCode  

    ★ Redirecionar a porta para SSH

<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/20a2994b-385f-4772-8441-d876841da964" width="500px" />   
</div>

    Instalar a extensão do SSH no VS
<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/59493c2f-d6f2-4640-9206-eae482905352" width="500px" />   
</div>


    ★ Iniciando as configurações da extensão, definimos o local do arquivo de configuração
<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/d0db5822-6129-460d-9fd9-6e9b1d25a6eb" width="500px" />   
</div>


    ★ Criamos as pastas e um arquivo de texto sem extensão com o nome “config”
<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/feab17be-60db-4c75-90df-0a93f3602ac7" width="500px" />   
</div>

    ★ Inserimos o comando para conectarmos ao ssh

<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/e75cb1ca-fc06-480e-8afa-c5ef8944fe9f" width="500px" />   
</div>


    ★ Conectamos e inserimos novamnete a senha a senha

<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/8ddbc337-8919-43f3-a3d3-4607bdb14c35" width="500px" />   
</div>


    ★ Apetamos Crtl+L para abrir o terminal

<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/cc740809-daac-4959-9160-25b658644f9a" width="500px" />   
</div>


---

### ☆ *Criando um arquivo Nasm 

    ★ Add a extensão de icon pra auxiliar 

<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/c08c8e48-f405-44de-8f4d-e06250f4d1fb" width="500px" />   
</div>

    ★ Criando o arquivo 

    ★ Comitando 

        ↳ *git commit -m “Criação de arquivo”

<img src="" width="500px" />   
</div>

#### ☆ Codando o arquivo 

    ★ comita-lo novamente 

<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/3c851b17-9741-41de-a10c-a74415b4b596" width="500px" />   
</div>

#### ☆ Com o comando 

    ↳ nasm -f elf hello.asm criamos o seu binario

<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/7ac9d60f-ec90-464e-81a1-42e892e34c81" width="500px" />   
</div>

---
<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/97bcac92-9421-49bc-a8ab-ec1efe80c940" width="500px" />   
</div>

    ld - link dynamic (comando do linux)
    Comando Linux ld. Nos sistemas operacionais do tipo Unix, o ld **é um vinculador**. Ele combina vários objetos compilados e arquivos compactados, realoca seus dados e vincula referências de símbolos. Normalmente, o último passo na compilação de um programa é executar o ld 
 
    -m → make
    elf_i386 → arquitetura. (i386 → 32Bits i64 → 64 bits)
    -o →Objeto.  (nome do arquivo)
 
    No total temos o arquivo hello, o binario desse arquivo “hello.o” e com o ld criamos um executavel com esses arquivos
 

<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/51c30d2a-5a93-4e63-8629-67cbc3a31d29" width="500px" />   
</div>

☆ Encaminhar para o git

<img src="https://github.com/fallsmeii/Aula-6/assets/149728744/1510df1b-6d0e-40e4-8337-8bd4ad9b19f6" width="500px" />   

>git push -u oringin main é utilizado quando queremos enviar a branch que criamos para o repositório remoto. Isso criará um “elo” entre o seu repositório local e o repositório remoto. 
