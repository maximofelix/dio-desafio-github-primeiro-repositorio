#GIT

//Cria a chave. Colocar no github(web)
ssh-keygen -t ed25519 -C xxxxxxx@gmail.com

// Start o serviço
eval $(ssh-agent -s)

//Associa a chave ao serviço
// entra na pasta
ssh-add id_ed25519

// Inicializa um repositório local
git init

// Clona um repositório
// entra na pasta onde ficará o repositorio
// pegar o caminho no repositorio do github
git remote add origin https://github.com/xxxxxxx/dio-desafio-github-primeiro-repositorio.git

// Obtem os dados do remote
git pull

// atualiza os dados no remote
git push

// No local, após alterar qualquer coisa na pasta
git add *

// Para ver o status do repositório
git status

// Para dar o commit localmente
git commit -m "Texto com descrição do Commit"