# Play Framework + Docker + AWS BeanStalk

Exemplo de como fazer o deploy de uma aplicação Play no ElasticBeanstalk.

A instrução do Dockerfile gera dois containers. 
O primeiro é usado para fazer o unzip da aplicação.
O segundo para executar a aplicação e ouvir na porta 9000.

O deploy da aplicação no Beanstalk pode ser feito através da linha de comando.

[Instalação do EB CLI](https://github.com/aws/aws-elastic-beanstalk-cli-setup)
[Configuração do EB CLI](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/eb-cli3-configuration.html)

Com o EB CLI instalado basta seguir os seguintes passos para testar local e publicar a aplição:

[Using the Docker platform](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/single-container-docker.html#single-container-docker.test-local)