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

	git shorlog -sn # mostra só a quantidades de commits e o nome da pessoa
	git log -graph # Mostra em forma grafica algumas coisas
	git show "hash" # Ex: 'git show 9283sn' 


# Outros Comandos II
	git diff # Usando para ver as modificações antes de se fazer commit //Importante
	git diff --name-only # Mostra o nome do arquivo modificado
	
	