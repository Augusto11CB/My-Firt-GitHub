Arquivo de Comandos Git e GitHub



Para Abrir o vi: vi Nome_do_Arquivo


# Comandos git

git status

subl Arquivo.kappa

git add Arquivo.kappa

git commit -m "Meu Comentario/MSG"


Tipos de Arquivos GitHub
	a. Untracked : Arquivo existe, mas não foi "visto" pelo git, ou seja, não existe nenhuma versão desse arquivo no repositório do git.
	b. Unmodified : Existe no git, mas não teve nenhuma modificação.
	c. Modified : o arquivo foi modificado, mas ainda não foi "salvo".
	d. Staged : Estágio que permite o arquivo ser salvo e portanto criar uma versão. Se o arquivo está nessa sessão e executarmos o comando "commit" o arquivo ficara com o tipo("b")

# Outros Comandos I
	git log
	git log --decorate
	git log --author="nome"
	git shortlog # mostra quais foram os autores, quantos commits fizeram e quais eles foram

	git shortlog -sn # mostra só a quantidades de commits e o nome da pessoa
	git log -graph # Mostra em forma grafica algumas coisas
	git show "hash" # Ex: 'git show 9283sn' 


# Outros Comandos II
	git diff # Usando para ver as modificações antes de se fazer commit //Importante

	git diff --name-only # Mostra o nome do arquivo modificado
	
	git checkout Nome.arq # Tira a ultima modificação 

	git reset HEAD # Comando 'git add Arq.name' dado, logo arquivo esta em 'Staged' para remove-lo desse estado (Motivo: "mudar a ultima edição, etc")


		--soft # retira do 'commit' e volta para o estágio 'Staged'

		--mixed # retira do 'commit' e volta para 'modified'

		-- hard # elimina tudo, até as edições

		help.github.com/articles/connecting-to-github-with-ssh
#################Git Hub################

https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/

após gerar a chave temos que

	cd ~/.ssh/

	cat id_rsa.pub

	Copiar chave gerada.

	Ir em github > setting > ssh and gpg keys e add a chave