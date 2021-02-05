# Tutorial RabbitMQ
RabbitMQ servidor de mensageria open source desenvolvido em Erlang.

# Utilizando imagem docker para criar um container para rodar o RabbitMQ local.

--Rodar o docker na sua máquina e já com o Docker rodando e configurado executar a aseguinte linha de comando

    docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3-management
 -Vai rodar na porta    
    http://localhost:15672/
    
 - Você pode acessar com usuario e senha padrão
      -> User :    guest
      -> Password: guest
   
#Após clonar o repositorio 

  https://github.com/LucasTroleiz/RabbitMQ.git

Você pode carregar o projeto na sua ide, e dentro dela executar os seguintes comandos.

    mvn clean package

Na pasta raiz rode o seguinte comando para rodar o sender
Utilize este para enviar, simplesmente executando o comando.

    java -jar target/RabbitMQ-0.0.1-SNAPSHOT.jar --spring.profiles.active=hello-world,sender

Na pasta raiz rode o seguinte comando para rodar o receiver
Utilize este para receber, simplesmente executando o comando.

    java -jar target/RabbitMQ-0.0.1-SNAPSHOT.jar --spring.profiles.active=hello-world,receiver


