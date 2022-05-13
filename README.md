# Gerar commits assinados ✅

1) **gpg --full-generate-key**

2) escolher RSA e configurar

3) **gpg —armor —export ID** (Para pegar o id, rodar o comando: **gpg --list-secret-key --keyid-form LONG** e pegar depois de rsaXXXX/)

4) copiar a chave pública e colocar no github (settings → GPG keys)

5) **git config --global user.signingkey ID** → pro git usar sua chave para assinar

6) exportar variável de ambiente **export GPG_TTY=$(tty)**

7) assinar commits por padrão **git config --global commit.gpgsign true** e **git config --global tag.gpgSign true**
