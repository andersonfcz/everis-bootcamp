
NDOWS 	LINUX
dir		ls
cd		cd
cls		clear	ctrl+ l
mkdir		mkdir
del /rmdir	rm / rmdir


BLOB
Objeto que representa cada arquivo rastreado pelo git. Cada blob possui uma chave hash que representa o estado atual do arquivo

TREE
Objeto que representa uma estrutura de diretorios rastreados pelo git. Cada tree aponta para os blobs contidos naquele diretorio blobs e outras arvores que representam os subdiretorios. Possui uma chave hash para representar o estado atual da arvore, como cada arvore é composta por outros blobs e arvores, uma modificação em qualquer numero desses objetos refletem no estado atual da arvore e por consequência em sua chave hash.

COMMIT
Objeto que representa um estado do repositorio. Composta por uma tree que é raiz do seu repositorio, autor, mensagem, timestamp e o commit anterior ao qual ele está relacionado. Possui uma chave hash que representa o estado atual do commit, modificações em sua tree ou nos blobs dessa tree, alteram seu estado e também sua chave hash.

git init
Comando usado para inicializar um repósitorio, ao utilizar este comando o git passa a rastrear quaisquer alterações que ocorram neste diretório.

UNTRACKED
Arquivos que se encontram no diretório inicializado pelo git, mas que ainda não estão sendo rastreados pelo git.
Ao utilizarmos o comando git add passamos a rastrear este arquivo e movemos ele para o estado staged.

UNMODIFIED
Estado que se encontram os arquivos já commitados.

MODIFIED
Estado dos arquivos após terem sidos modificados. Ao modificarmos um arquivo utilizamos o comando git add para movermos estas modificações para o estado staged.

STAGED
Estado onde os arquivos se encontram prontos para serem commitados e serem enviados para o repositorio local.


WORKING DIRECTORY
Arquivos untracked e modified

STAGING AREA
Arquivos prontos para serem commitados

LOCAL REPOSITORY
Arquivos commitados.

REMOTE REPOSITORY.
Servidor remoto, contendo commits enviados por diferentes mantenedores.


