```
// baixe e obtenha detalhes das imagens em (https://hub.docker.com/) 
 
docker run nome_imagem comando // roda ou baixa a imagem desejada e executa o comando a partir dela 
--name nome_desejado //apelido para o container 
-e VARIAVEL_AMBIENTE=valor_variavel // seta variável ambiente 
--link alias_container_relacionado:nome_real 
-d // roda em background 
-p //porta de um container e do outro linkado 
-i // interativa com o shell do container  
-t // simula o TTY 
--rm // faz com que o container seja descartado ao fim da interação 
 
docker pull // faz o pull (como no git) da imagem do sistema 
 
docker images // lista as imagens baixadas 
 
docker ps // lista os containes rodando 
-a // lista incluindo containers parados 
-q // exibe somente números dos ids 
 
docker start nome_container // inicia um container parado anteriormente 
 
docker exec nome_do_container comando 
-i // interativa com o shell do container  
-t // simula o TTY 
  
docker rm nome_container // remove o container, não a imagem 
 
docker stop nome_container // para o container 
 Ou $(docker ps -qa) // no lugar do nome do container, esse comando remove todos os containers 
 
docker rmi nome_imagem // remove a imagem e suas camadas 
 
docker kill nome_container // força saída do container
```