# Notas Aulas - Introdução ao Git e GitHub :book:



**Git** - Criar e monitorar diferentes versões de códigos. Navegação via *Command Line Interface*.

Para utilizar o Git Bash e o GitHub de forma segura deve-se gerar *chave de segurança*. Dois métodos são disponibilizados:

* **Tokens** - Gerado no GitHub. Deve-se guardar o conteúdo da chave, pois só é mostrada pelo GitHub um única vez. A chave é necessária para cada alterações feitas nos repositórios.

* **SSH** - São geradas duas chaves (uma pública e outra privada) no Git Bash. Comandos importantes:

  * ###### ssh-keygen -t ed25519 -C (inserir e-mail GitHub)

    * Cadastrar senha. 

  * ###### cat id_ed25519.pub

    * Visualizar chave pública gerada.  Copiar a chave pública para ser cadastrada no GitHub > SSH keys. 

​		A chave privada deve ser cadastrada no Git Bash para ser administrada. Comandos importantes:	

* ###### eval $ (ssh-agent -s)

  * A saída será o número de start do projeto.

* ###### ssh-add id_ed25519

  * A chave privada será passada para o agent administrar. Deve-se confirmar com a senha cadastrada.

  Após esse processo o protocolo SSH estará instalado na máquina e poderá ser utilizada a chave SSH na clonagem de repositórios.



