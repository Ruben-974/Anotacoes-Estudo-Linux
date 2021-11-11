# [*Curso Linux*](https://www.youtube.com/playlist?list=PLnDvRpP8BnezDTtL8lm6C-UOJZn-xzALH) 
Agradecimento a Matheus Battisti do canal [Hora de Codar](https://www.youtube.com/channel/UCDoFiMhpOnLFq1uG4RL4xag)
## [*Aula #04*](https://www.youtube.com/watch?v=I6jWfLEG7kk&list=PLnDvRpP8BnezDTtL8lm6C-UOJZn-xzALH&index=4) - Mudando diretórios (Comando cd)

Comando cd - Usado para mudarmos diretórios no terminal, ir e voltar onde quiser no diretório

Podemos ir diretamente para onde queremos se soubermos o caminho específico do diretorio desejado

Estamos na raiz e vamos ir até a pasta 'Música' do usuario

`cd home/user/Música`

Estamos no diretório `home/user/Música` de exemplo:

`cd ..` - Diretorio anterior

Se usarmos `cd ..` irá para `home/user` usando `cd ..` novamente iremos para `home`

Podemos usar `cd ../..` para voltar 2 diretorios, caso queira voltar 3 diretórios adicione mais um `/..`, assim sucessivamente

Outras informações interresantes 

`cd .` - Diretório atual

Em `user@pc:~$` o ' ~ ' significa que estamos na pasta principal do usuario
Podemos usar `cd ~` para irmos direto para essa pasta

De forma semelhante ao ' ~ ' a ' / ' em `user@pc:/$` também funciona assim, porém significa a raiz

## [*Aula #05*](https://www.youtube.com/watch?v=QXJ6_4HPx5Q) - Listando / exibindo arquivos e diretórios (Comando ls)

Se estivermos no diretório do usuario e usarmos ls, irá listar os arquivos e diretorios dessa pasta

- `ls` - Usado para listar ou exibir arquivos no diretório

`Downloads   Modelos   Público   Vídeos   Documentos   Imagens   Música`

Alguns parametros para `ls`

- `ls -l` - Faz uma listagem mais detalhada dos itens no diretório

```
   drwxr-xr-x 5 user user 4096 out 22 01:24  Documentos
   drwxr-xr-x 3 user user 4096 out 22 11:56  Downloads
   drwxr-xr-x 3 user user 4096 out 22 00:59  Imagens
   drwxr-xr-x 2 user user 4096 out 21 17:49  Modelos
   drwxr-xr-x 7 user user 4096 out 21 19:37  Música
   drwxr-xr-x 2 user user 4096 out 21 17:49  Público
   drwxr-xr-x 2 user user 4096 out 22 01:07  Vídeos
```

- `ls -a` - Mostra diretorios e arquivos ocultos (que começam com ' . ')

`Downloads   Modelos   Público   Vídeos   Documentos   Imagens   Música   .local   .config`

Também podemos unir parametros

- `ls -la` - Irá mostras uma lista detalhada com os arquivos acultos

```
   drwxr-xr-x 5 user user 4096 out 22 01:24  Documentos
   drwxr-xr-x 3 user user 4096 out 22 11:56  Downloads
   drwxr-xr-x 3 user user 4096 out 22 00:59  Imagens
   drwxr-xr-x 2 user user 4096 out 21 17:49  Modelos
   drwxr-xr-x 7 user user 4096 out 21 19:37  Música
   drwxr-xr-x 2 user user 4096 out 21 17:49  Público
   drwxr-xr-x 2 user user 4096 out 22 01:07  Vídeos
   drwxr-xr-x 3 user user 4096 out 21 17:49  .local
   drwx------ 23 user user 4096 out 22 11:41  .config

```

- `ls -h` - Irá mostrar o tamanho dos arquivos de uma forma mais "legivel" | Obs: Use `ls -lh` pois somente o `-h` não será possivel a vizualização

```
   drwxr-xr-x 5 user user 4,0K out 22 01:24  Documentos
   drwxr-xr-x 3 user user 4,0K out 22 11:56  Downloads
   drwxr-xr-x 3 user user 4,0K out 22 00:59  Imagens
   drwxr-xr-x 2 user user 4,0K out 21 17:49  Modelos
   drwxr-xr-x 7 user user 4,0K out 21 19:37  Música
   drwxr-xr-x 2 user user 4,0K out 21 17:49  Público
   drwxr-xr-x 2 user user 4,0K out 22 01:07  Vídeos
```

- `ls -lha` - Mostra a lista detalhada + tamanhos dos arquivos mais "legivel" + Arquivos ocultos

```
   drwxr-xr-x 5 user user 4,0K out 22 01:24  Documentos
   drwxr-xr-x 3 user user 4,0K out 22 11:56  Downloads
   drwxr-xr-x 3 user user 4,0K out 22 00:59  Imagens
   drwxr-xr-x 2 user user 4,0K out 21 17:49  Modelos
   drwxr-xr-x 7 user user 4,0K out 21 19:37  Música
   drwxr-xr-x 2 user user 4,0K out 21 17:49  Público
   drwxr-xr-x 2 user user 4,0K out 22 01:07  Vídeos
   drwxr-xr-x 3 user user 4,0K out 21 17:49  .local
   drwx------ 23 user user 4,0K out 22 11:41  .config
```

- `ls -tr` - Ordena os arquivos pela data de modificação

```
drwxr-xr-x 2 user user 4096 out 21 17:49  Público
drwxr-xr-x 2 user user 4096 out 21 17:49  Modelos
drwxr-xr-x 7 user user 4096 out 21 19:37  Música
drwxr-xr-x 3 user user 4096 out 22 00:59  Imagens
drwxr-xr-x 2 user user 4096 out 22 01:07  Vídeos
drwxr-xr-x 5 user user 4096 out 22 01:24  Documentos
drwxr-xr-x 3 user user 4096 out 22 11:56  Downloads
```

Por fim, podemos listar outros diretorios sem ter que usar o cd para listar o diretório desejado apenas dizendo o diretório após os parâmetros

- `ls -l /var/`

Irá retornar uma lista detalhada dos arquivos da pasta var

## [*Aula #06*](https://www.youtube.com/watch?v=YZyuUM-4AnQ) - Limpando a tela do terminal (Comando clear)

O comando `clear` basicamente limpa a tela do terminal, nada de especial alem disso, podemos usar o atalho ctrl + l para "limpar" o terminal, esse atalho somente pula algumas linhas para deixar o terminal mais limpo, mas os comando antigos continuam lá

## [*Aula #07*](https://www.youtube.com/watch?v=6o1ucZJNXuc&list=PLnDvRpP8BnezDTtL8lm6C-UOJZn-xzALH&index=7&t=1s) - Visualizando arquivos no terminal (Comando cat)

O comando `cat` serve basicamente para visualizar arquivos, com o comando `cat` você pode visulizar arquivos .txt pelo terminal, ou até outros arquivos como .py .js .html .css etc

Suponhamos que você irá abir um arquivo .txt chamado "exemplo.txt" e nele tem o conteudo "Olá, Mundo!"
usando `cat exemplo.txt` irá retonrar "Olá, Mundo!"

Tembém podemos abrir 2 arquvivos concatenados, criemos o arquivo "exemplo2.txt" seu conteuso será "Arquivo de exemplo número 2"

Usando `cat exemplo.txt exemplo2.txt` retornará:

"

Olá, Mundo!

Arquivo de exemplo número 2

"

Podemos usar o mesmo arquivo se desejado `cat exemplo.txt exemplo.txt`

"

Olá, Mundo!

Olá, Mundo!

"

Podemos criar um arquivo concatenado usando o > vejamos `cat exemplo.txt exemplo2.txt > junção.txt`

"junção.txt" será criado, quando visualizado (`cat junção.txt`) irá mostrar:

"

Olá, Mundo!

Arquivo de exemplo número 2

"

Podemos criar arquivos usando o comando `cat > nome_do_arquivo.txt`, apesar de não ser a forma mais adequada para isso, vocẽ poderá digitar e quando finalizado use Ctrl + C para finalizar a digitação do documento

podemos usar o parâmetro -n para mostrar as linhas do aquivo, exemploe: `cat -n junção.txt`

"

1  Olá, Mundo!

2  Arquivo de exemplo número 2

"

## [*Aula #08*](https://www.youtube.com/watch?v=5MF26dcT2J8&list=PLnDvRpP8BnezDTtL8lm6C-UOJZn-xzALH&index=8) - Criando arquivos (Comando touch)

O comando touch serve para criar um arquivo ou atualizar a data de modificação

Criando um arquivo `touch teste.txt` o arquivo "teste.txt"

Suponhamos que temos um arquivo chamado "antigo.txt" e queremos atualizar a sua data de modificação, foi então use `touch antigo.txt`
