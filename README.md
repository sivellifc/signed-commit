Habilita assinatura no repositório: git config commit.gpgsign true

Cria chave: gpg --full-generate-key

Lista chaves (pegar ID): pg --list-secret-keys --keyid-format=long

Gera chave pública: gpg --armor --export 60AFC2230352B836

Editar chave: gpg --edit-key 60AFC2230352B836

	Adicionar outro email: adduid

COnfigura key no git: git config user.signingkey 60AFC2230352B836


Agent:

	- Adicionar use-agent em ~/.gnupg/gpg.conf
	- gpgconf --launch gpg-agent



