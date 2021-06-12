git config --global user.name <nome>
git config --global user.email <email>
git config --global core.editor <vscode>

git init
git add -A
Adiciona todos os arquivos modificados/criados para o staging area.

git add index.html
Adiciona o arquivo específico para o staging area.

git commit -m "Message"
Faz commit dos arquivos com a mensagem, parâmetro -m.

git commit -am "Message"
Faz commit dos arquivos junto com o comando git add -A.

git status
Mostra os arquivos untracked e preparados para commit.

git log
Mostra os commits realizados naquele branch.

git reset --soft <codigo commit>
Move o HEAD para o commit indicado, sem mudar o working dir e o staging area. (Não altera os conteúdos dos arquivos, somente volta o commit para o indicado, para fazer as alterações novamente).

git reset --mixed <codigo commit>
Parâmetro padrão
Move o HEAD para o commit indicado, atualiza o staging area com o conteúdo que está nesse commit.

git reset --hard <codigo commit>
Move o HEAD para o commit indicado, atualiza tanto o staging area quanto o working dir.

git branch <nome>
Cria um novo branch.

git checkout <nome>
Troca o branch apartir do branch atual.

git checkout -b <nome>
Cria e troca para a branch criada, partindo do branch atual.

git checkout HEAD -- <nome do arquivo>
Remove um arquivo
HEAD: Preenche com o nome do branch atual

git diff
Ver as diferenças dos commits, mostra o código com as modificações.

git diff --name-only
Ver as diferenças dos commits, somente os nomes dos arquivos.

git diff <arquivo>
Ver as diferenças de um arquivo específico.

git revert --no-edit <codigo commit a ser revertido>
Reverte o commit e os arquivos.

git branch -D <nome do branch>
Deletar o branch no local.

git push origin :<nome>
Deletar o branch e todas suas modificações no remoto.

git ls-files -s
Ver oque está em staging area (pronto para ser enviado ao servidor remoto)

git cat-file -p <hash do arquivo>
Ver o conteúdo do arquivo

git push origin <branch>
Envia os arquivos local para o servidor remoto, baseado no branch indicado.

git pull origin <branch>
Puxa os arquivos/histórico do servidor remoto para o local, no branch indicado.