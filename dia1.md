Dia 1: Introdução ao Go
=======================

Introdução
----------

Neste tutorial de uma semana, você aprenderá o básico da linguagem de programação Go. Go é uma linguagem de programação compilada, desenvolvida pelo Google, que possui uma sintaxe clara e concisa, além de recursos de concorrência e eficiência de alto desempenho.

Este tutorial foi projetado para desenvolvedores Java que desejam aprender Go e já possuem experiência em programação orientada a objetos e em uma linguagem de programação com tipagem estática, como Java. É útil, mas não necessário, ter conhecimentos prévios em linguagens de programação compiladas, como C/C++.

Preparação
----------

Antes de começarmos, você precisará instalar o Go em sua máquina. Você pode baixar a última versão estável do Go em [https://golang.org/dl/](https://golang.org/dl/). Certifique-se de seguir as instruções de instalação apropriadas para o seu sistema operacional.

Após a instalação, verifique se o Go está funcionando executando o seguinte comando no terminal:

```shellscript
go version
```

Isso deve retornar a versão do Go que você acabou de instalar.

Configuração do ambiente
------------------------

Depois de instalar o Go, é hora de configurar o ambiente de desenvolvimento. Crie uma pasta para o seu projeto e configure o caminho GOPATH para apontar para esta pasta. GOPATH é a variável de ambiente que especifica o caminho raiz do diretório de trabalho do Go.

```shellscript
    mkdir myproject
    export GOPATH=$(pwd)/myproject
```

Isso criará uma pasta chamada `myproject` e definirá o GOPATH para o caminho absoluto da pasta atual + "/myproject".

Primeiros passos
----------------

Agora que temos tudo configurado, podemos começar a escrever código em Go. Vamos começar com um programa muito simples que imprime "Hello, World!" na saída padrão.

### Criando um arquivo Go

Abra seu editor de texto favorito e crie um arquivo chamado `main.go` na pasta do seu projeto. Para iniciarmos, escrevemos o código abaixo no arquivo:

```golang
package main

import "fmt"

func main() {
    fmt.Println("Hello, World!")
}
```

O primeiro comando do arquivo é o `package main`, que declara que este é um pacote executável. Isso significa que podemos executar esse código diretamente sem precisar compilar bibliotecas primeiro.

Em seguida, importamos o pacote `fmt`, que nos permitirá formatar e imprimir texto na saída padrão.

Por fim, temos a função `main`, que é o ponto de entrada para o nosso programa. Dentro desta função, chamamos a função `Println` do pacote `fmt`, que imprime o texto "Hello, World!" na saída padrão.

### Compilando e executando o programa

Para executar o nosso programa, basta executar o seguinte comando no terminal:

```shellscript
go run main.go
```

Isso compilará e executará o nosso programa, imprimindo "Hello, World!" na saída padrão.

Se preferir, você também pode compilar o programa em um arquivo executável. Para fazer isso, execute o seguinte comando:

```shellscript
go build main.go
```

Isso criará um arquivo executável chamado `main` na pasta do seu projeto. Para executar o arquivo, basta executar o seguinte comando:

```
./main
```    

Parabéns! Você acabou de escrever e executar seu primeiro programa em Go.

Conclusão
---------

Neste primeiro dia, você aprendeu o básico da linguagem de programação Go, instalou o Go em sua máquina, configurou o ambiente de desenvolvimento e escreveu e executou seu primeiro programa em Go. Nos próximos dias, continuaremos a explorar a linguagem Go em mais detalhes.
