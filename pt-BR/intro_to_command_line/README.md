# Introdução à linha de comando

> Para os leitores em casa: este capítulo é coberto no vídeo [ Seu novo amigo: linha de comando ](https://www.youtube.com/watch?v=jvZLWhkzX-8).

É emocionante, não?! Você vai escrever sua primeira linha de código em poucos minutos! :)

**Deixe-nos apresentá-lo ao seu primeiro novo amigo: a linha de comando!**

As etapas a seguir mostraram a você como usar a janela preta que todos os hackers usam. Pode parecer um pouco assustador no começo, mas realmente é apenas um prompt esperando por comandos de você.

> **Nota** Note que ao longo deste livro intercalamos o uso dos termos 'diretório' e 'pasta', mas eles significam a mesma coisa.

## O que é a linha de comando?

A janela, que geralmente é chamada de **linha de comando** ou **interface de linha de comando**, é uma aplicação de texto para ver e manipular arquivos de seu computador. É como se fosse o Windows Explorer ou o Finder no Mac, porém sem a interface gráfica. Outros nomes para a linha de comando são: *cmd*, *CLI*, *prompt*, *console* ou *terminal*.

## Abra a interface de linha de comando

Para começar alguns experimentos, precisamos abrir a nossa interface de linha de comando primeiro.

<!--sec data-title="Opening: Windows" data-id="windows_prompt" data-collapse=true ces-->

Vá para o Menu iniciar → Sistema do Window → Prompt de comando.

> Em versões antigas do windows, procure em Menu iniciar → Todos programas → Acessórios → Prompt de comando.

<!--endsec-->

<!--sec data-title="Opening: OS X" data-id="OSX_prompt" data-collapse=true ces-->

Vá para Aplicações → Utilidades → Terminal.

<!--endsec-->

<!--sec data-title="Opening: Linux" data-id="linux_prompt" data-collapse=true ces-->

Provavelmente você vai achar em Aplicativos → Acessórios → Terminal, mas isso depende do seu sistema operacional. Qualquer coisa é só procurar no Google. :)

<!--endsec-->

## Prompt

Agora você deve ver uma janela branca ou preta que está à espera de seus comandos.

<!--sec data-title="Prompt: OS X and Linux" data-id="OSX_Linux_prompt" data-collapse=true ces-->

Se você estiver em Mac ou num Linux, você provavelmente verá um `` $, como este:

{% filename %}command-line{% endfilename %}

    $
    

<!--endsec-->

<!--sec data-title="Prompt: Windows" data-id="windows_prompt2" data-collapse=true ces-->

No Windows, é um sinal de `>`, como este:

{% filename %}command-line{% endfilename %}

    >
    

<!--endsec-->

Cada comando será antecedido por este sinal e um espaço, mas você não precisa digitá-lo. Seu computador fará isso por você. :)

> Uma pequena observação: no nosso caso existe algo como `C:\Users\ola>` ou `Olas-MacBook-Air:~ ola$` antes do cursor e isso está 100% correto.

A parte até e incluindo o `$` ou o `>` é chamada de *prompt de linha de comando*, ou *prompt* de forma breve. Ele solicita que você de a entrada de algo.

No tutorial, quando queremos que você digite um comando, nós incluiremos o `$` ou `>` e por vezes até mais para a esquerda. Você pode ignorar a parte esquerda e apenas digite o comando que inicia após o prompt.

## Seu primeiro comando (Uhuu!)

Vamos começar digitando este comando:

<!--sec data-title="Your first command: OS X and Linux" data-id="OSX_Linux_whoami" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    $ whoami
    

<!--endsec-->

<!--sec data-title="Your first command: Windows" data-id="windows_whoami" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    > whoami
    

<!--endsec-->

E em então aperte `enter`. Este é o nosso resultado:

{% filename %}command-line{% endfilename %}

    $ whoami
    olasitarska
    

Como você pode ver o computador acabou de mostrar seu nome de usuário na tela. Legal, né? :)

> Tente escrever cada comando, não copie e cole. Você vai se lembrar melhor dos comandos desse jeito!

## O Básico

Cada sistema operacional tem o seu próprio conjunto de instruções para a linha de comando, então se certifique que você está seguindo as instruções do seu sistema operacional. Vamos tentar, certo?

### Pasta atual

Seria legal se soubéssemos em que diretório estamos, certo? Para isso, digite o seguinte comando e aperte `enter`:

<!--sec data-title="Current directory: OS X and Linux" data-id="OSX_Linux_pwd" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    $ pwd
    /Users/olasitarska
    

> Nota: 'pwd' significa 'print working directory' (imprima/mostre o diretório de trabalho).

<!--endsec-->

<!--sec data-title="Current directory: Windows" data-id="windows_cd" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    > cd
    C:\Users\olasitarska
    

> Nota: 'cd' significa 'change directory' em inglês, o que se traduz para 'mudar de diretório'. Com o powershell, você pode utilizar pwd da mesma forma como no Linux ou Mac OS X.

<!--endsec-->

Você provavelmente vai ver algo parecido em seu computador. A linha de comando geralmente inicia no diretório principal do usuário, também chamado de diretório "home", em Inglês.

* * *

### Listando arquivos e pastas

Então o que tem nele? Seria legal descobrir. Vamos ver:

<!--sec data-title="List files and directories: OS X and Linux" data-id="OSX_Linux_ls" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    $ ls
    Applications
    Desktop
    Downloads
    Music
    ...
    

<!--endsec-->

<!--sec data-title="List files and directories: Windows" data-id="windows_dir" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    > dir
     Directory of C:\Users\olasitarska
    05/08/2014 07:28 PM <DIR>      Applications
    05/08/2014 07:28 PM <DIR>      Desktop
    05/08/2014 07:28 PM <DIR>      Downloads
    05/08/2014 07:28 PM <DIR>      Music
    ...
    

> Nota: No powershell, você também pode usar 'ls' como no Linux e Mac OS X. <!--endsec-->

* * *

### Entrar em outra pasta

Agora, vamos para a pasta Desktop:

<!--sec data-title="Change current directory: OS X and Linux" data-id="OSX_Linux_move_to" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    $ cd Desktop
    

<!--endsec-->

<!--sec data-title="Change current directory: Windows" data-id="windows_move_to" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    > cd Desktop
    

<!--endsec-->

Veja se realmente entramos na pasta:

<!--sec data-title="Check if changed: OS X and Linux" data-id="OSX_Linux_pwd2" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    $ pwd
    /Users/olasitarska/Desktop
    

<!--endsec-->

<!--sec data-title="Check if changed: Windows" data-id="windows_cd2" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    > cd
    C:\Users\olasitarska\Desktop
    

<!--endsec-->

Aqui está!

> Dica de profissional: se você digitar `cd D` e apertar a tecla `tab` no seu teclado, a linha de comando irá preencher automaticamente o resto do nome para que você possa navegar rapidamente. Se houver mais de uma pasta que comece com "D", aperte a tecla `tab` duas vezes para obter uma lista de opções.

* * *

### Criando uma pasta

Que tal criar um diretório em sua área de trabalho para praticarmos? Você pode fazer isso com o seguinte comando:

<!--sec data-title="Create directory: OS X and Linux" data-id="OSX_Linux_mkdir" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    $ mkdir practice
    

<!--endsec-->

<!--sec data-title="Create directory: Windows" data-id="windows_mkdir" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    > mkdir practice
    

<!--endsec-->

Esse pequeno comando criará um diretório chamado `practice` em sua área de trabalho. Você pode verificar se o diretório realmente está lá olhando sua área de trabalho ou executando o comando `ls` ou `dir`! Experimente. :)

> Dica de profissional: Se você não quiser digitar o mesmo comando várias vezes, tente pressionar `seta para cima` e `seta para baixo` no teclado para percorrer comandos usados recentemente.

* * *

### Exercite-se!

Um pequeno desafio para você: crie um diretório dentro do diretório `practice` chamando `test`. (Use os comandos `cd` e `mkdir`.)

#### Solução:

<!--sec data-title="Exercise solution: OS X and Linux" data-id="OSX_Linux_test_dir" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    $ cd practice
    $ mkdir test
    $ ls
    test
    

<!--endsec-->

<!--sec data-title="Exercise solution: Windows" data-id="windows_test_dir" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    > cd practice
    > mkdir test
    > dir
    05/08/2014 07:28 PM <DIR>      test
    

<!--endsec-->

Parabéns! :)

* * *

### Limpando

Não queremos deixar uma bagunça, então vamos remover tudo o que fizemos até agora.

Primeiro, precisamos voltar para a pasta Desktop:

<!--sec data-title="Clean up: OS X and Linux" data-id="OSX_Linux_back" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    $ cd ..
    

<!--endsec-->

<!--sec data-title="Clean up: Windows" data-id="windows_back" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    > cd ..
    

<!--endsec-->

Ao utilizar o `..` junto com o comando `cd` você muda o diretório atual para o diretório pai (o diretório que contém o seu diretório atual).

Veja onde você está:

<!--sec data-title="Check location: OS X and Linux" data-id="OSX_Linux_pwd3" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    $ pwd
    /Users/olasitarska/Desktop
    

<!--endsec-->

<!--sec data-title="Check location: Windows" data-id="windows_cd3" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    > cd
    C:\Users\olasitarska\Desktop
    

<!--endsec-->

Agora é hora de deletar o diretório `pratice`:

> **Atenção**: A exclusão de arquivos usando `del`, `rmdir` ou `rm` é irreversível; ou seja, os *arquivos excluídos são perdidos para sempre*! Então, tenha cuidado com este comando.

<!--sec data-title="Delete directory: Windows Powershell, OS X and Linux" data-id="OSX_Linux_rm" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    $ rm -r practice
    

<!--endsec-->

<!--sec data-title="Delete directory: Windows Command Prompt" data-id="windows_rmdir" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    > rmdir /S practice
    practice, Are you sure <Y/N>? Y
    

<!--endsec-->

Pronto! Para ter certeza que a pasta foi excluída, vamos checar:

<!--sec data-title="Check deletion: OS X and Linux" data-id="OSX_Linux_ls2" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    $ ls
    

<!--endsec-->

<!--sec data-title="Check deletion: Windows" data-id="windows_dir2" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    > dir
    

<!--endsec-->

### exit

Isso é tudo, por enquanto! Agora você pode fechar a janela do terminal, mas vamos fazer do jeito hacker, né? :)

<!--sec data-title="Exit: OS X and Linux" data-id="OSX_Linux_exit" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    $ exit
    

<!--endsec-->

<!--sec data-title="Exit: Windows" data-id="windows_exit" data-collapse=true ces-->

{% filename %}command-line{% endfilename %}

    > exit
    

<!--endsec-->

Legal, né? :)

## Sumário

Aqui vai uma lista de alguns comandos úteis:

| Comando (Windows) | Comando (Mac OS / Linux) | Descrição                     | Exemplo                                           |
| ----------------- | ------------------------ | ----------------------------- | ------------------------------------------------- |
| saindo            | saindo                   | Fecha a janela                | **saindo**                                        |
| cd                | cd                       | Muda a pasta                  | **cd test**                                       |
| cd                | pwd                      | mostra o diretório atual      | **cd** (Windows) ou **pwd** (Mac OS / Linux)      |
| dir               | ls                       | Lista as pastas e/ou arquivos | **dir**                                           |
| copy              | cp                       | Copia um arquivo              | **copy c:\test\test.txt c:\windows\test.txt** |
| move              | mv                       | Move um arquivo               | **move c:\test\test.txt c:\windows\test.txt** |
| mkdir             | mkdir                    | Cria uma pasta                | **mkdir testdirectory**                           |
| rmdir (ou del)    | rm                       | Exclui arquivo                | **del c:\test\test.txt**                        |
| rmdir /S          | rm -r                    | Exclui diretório              | **rm -r testdirectory**                           |

Esses são apenas alguns dos comandos que você pode rodar na sua linha de comando, porém não vamos usar mais do que isso hoje.

Se você estiver curioso, [ss64.com](http://ss64.com) contém uma referência completa de comandos para todos os sistemas operacionais.

## Pronto?

Vamos mergulhar no Python!