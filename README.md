# Tutorial RabbitMQ
RabbitMQ servidor de mensageria open source desenvolvido em Erlang.

# Utilizando imagem docker para criar um container para rodar o RabbitMQ local.

--Rodar o docker na sua máquina e já com o Docker rodando e configurado executar a aseguinte linha de comando

    docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3-management
 -Vai rodar na porta    
    http://localhost:15672/
    
 - Você pode acessar com usuario e senha padrão
      User :    guest
      Password: guest

