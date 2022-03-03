Habilita assinatura no repositório: git config commit.gpgsign true

Habilita assinatura das tags: git config tag.gpgSign true

Cria chave: gpg --full-generate-key

Lista chaves (pegar ID): gpg --list-secret-keys --keyid-format=long

Gera chave pública: gpg --armor --export 60AFC2230352B836

Editar chave: gpg --edit-key 60AFC2230352B836

	Adicionar outro email: 
		-adduid
	
	Marcar como confiável:
		- uid N ---> seleciona a uid. N é o número
		- trust
		- 5
		

COnfigura key no git: git config --global user.signingkey 60AFC2230352B836

Verificar assinatura:
- git log --show-signature -1

Agent:
	- export GPG_TTY=$(tty)
	- .bash_profile
	- Adicionar use-agent em ~/.gnupg/gpg.conf
	- gpgconf --launch gpg-agent



