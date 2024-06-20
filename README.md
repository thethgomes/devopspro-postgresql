# Desafio 01 - Banco de Dados Postgresql <h1>

>Você está dando os primeiros passos no uso de containers. E a melhor forma de iniciar no mundo de containers é usar em ambiente de desenvolvimento.
>Sua missão é ajudar a equipe de desenvolvimento a ter mais autonomia no desenvolvimento de projetos. E uma das reclamações da equipe é o setup local.
>Crie um comando para criar um banco de dados PostgreSQL no ambiente do desenvolvedor de uma forma que cumpra os seguintes requisitos:
>* O nome do banco de dados deve ser curso_docker
>* O usuário de acesso ao banco deve ser docker_usr
>* A senha do usuário deve ser docker_pwd
>  Lembrando que a execução em container deve ser transparente pra quem está desenvolvendo. E que aqui você não precisa se preocupar com a perda dos dados do banco e nem nada disso, é apenas para desenvolvimento pontual.

Coloque aqui embaixo o comando que a equipe deve usar pra criar um banco de dados PostgreSQL com esses requisitos:


~~~
docker container run -d -p 5432:5432 -e POSTGRES_DB=curso_docker -e POSTGRES_USER=docker_usr -e POSTGRES_PASSWORD="docker_pwd" postgres
~~~

