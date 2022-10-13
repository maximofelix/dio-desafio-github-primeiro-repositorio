#GIT

//Cria a chave. Colocar no github(web)
ssh-keygen -t ed25519 -C xxxxxxxxx@gmail.com

// Start o serviço
eval $(ssh-agent -s)

//Associa a chave ao serviço
// entra na pasta
ssh-add id_ed25519

// Inicializa um repositório local
git init

// Clona um repositório
git remote add origin https://github.com/maximofelix/dio-desafio-github-primeiro-repositorio.git
