# Bash terminal

## Cenário
* Para os exemplos a seguir, usaremos um diretório com a seguinte estrutura:

```
└───Example
    │   Notes.txt
    │
    ├───Games
    │       Space Invaders.exe
    │
    └───Pictures
            Selfie.png
```

## Navegação
* O bash pode ser aberto pelo iniciar > Git Bash ou clicando com o direito em qualquer diretório > Git Bash Here
    * Quando aberto pelo iniciar, o Bash inicializa no diretório **home**, que é o diretório do usuário atual, indicado por `~`.

        ```bash
        Darkangel@Dark-PC MINGW64 ~
        ```

    * Quando aberto em outro diretório, o Bash inicializa neste.

        ```bash
        Darkangel@Dark-PC MINGW64 ~/Desktop/Example
        ```

### ls [dirPath]
* Abreviação para list, **ls** lista o conteúdo da pasta atual se usado sozinho.

    ```bash
    Darkangel@Dark-PC MINGW64 ~/Desktop/Example
    $ ls
    Games/  Notes.txt  Pictures/
    ```

* Se usado com **dirPath**, lista o conteúdo da pasta **dirPath**, que deve estar contida na pasta atual.

    ```bash
    Darkangel@Dark-PC MINGW64 ~/Desktop/Example
    $ ls Pictures
    Selfie.png
    ```

### start .
* Inicializa o diretório atual com o explorer

![[start.png]]
### pwd
* Abreviação para **print working directory**, exibe o diretório atual completo.

    ```bash
    Darkangel@Dark-PC MINGW64 ~/Desktop/Example
    $ pwd
    /c/Users/Darkangel/Desktop/Example
    ```

### cd dirPath|..
* Pode entrar no diretório `dirPath`, que pode estar dentro do diretório atual ou ser outro diretório.
* Pode voltar um diretório com `..`

    ```bash
    Darkangel@Dark-PC MINGW64 ~/Desktop/Example
    $ cd games

    Darkangel@Dark-PC MINGW64 ~/Desktop/Example/games
    $ cd ..

    Darkangel@Dark-PC MINGW64 ~/Desktop/Example
    ```

### clear
* Limpa o terminal

## Criação e remoção de arquivos e diretórios

### mkdir dir [dirs]
* Cria um ou múltiplos diretórios
* Pode-se especificar o caminho onde serão criados

    ```bash
    mkdir Music
    mkdir Music/Classic
    ```

### touch file [files]
* Cria um ou múltiplos arquivos
* Pode-se especificar o caminho onde serão criados

    ```bash
    touch moreNotes.txt documentation.pdf
    ```

### rm file [files]
* Remove um ou múltiplos arquivos
* Pode-se especificar o caminho onde serão removidos

### rm -rf folder [folders]
* Remove um ou múltiplos diretórios
* Pode-se especificar o caminho onde serão removidos