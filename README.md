# [*Curso Linux*](https://www.youtube.com/playlist?list=PLnDvRpP8BnezDTtL8lm6C-UOJZn-xzALH) 
## [*Aula #04*](https://www.youtube.com/watch?v=I6jWfLEG7kk&list=PLnDvRpP8BnezDTtL8lm6C-UOJZn-xzALH&index=4) - Mudando diretórios (Comando cd)

Comando cd - Usado para mudarmos diretórios no terminal, ir e voltar onde quiser no diretório

- `cd .` - Diretório atual
- `cd ..` - Diretorio anterior

Podemos usar `cd ../..` para voltar 2 diretorios, caso queira voltar 3 diretórios adicione mais um `/..`, assim sucessivamente

Estamos no diretório `user@pc:~$` de exemplo:

- Se usarmos `cd ..` irá para `user@pc:/home$` que e a pasta 'home' da raiz, usando `cd ..` novamente iremos para a raiz `user@pc:/$`

Também podemos ir diretamente para onde queremos se soubermos o caminho específico do diretorio desejado

Estamos na raiz e vamos ir até a pasta 'Música' do usuario

- `cd home/user/Música`

Detalhes

- `user@pc:~$` o ' ~ ' significa que estamos na pasta principal do usuario
   - Podemos usar `cd ~` para irmos direto para essa pasta

- De forma semelhante o ' / ' em `user@pc:/$` também funciona assim, porém significa a raiz

