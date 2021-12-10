# Spring Web Flux - Criando gerenciamento de Herois 

Neste projeto desenvolvido através do Bootcamp promovido pela [TQI](https://www.linkedin.com/company/tqi-it/) - TQI Java Developers em parceria com a [Digital Innovation One](https://www.linkedin.com/school/digitalinnovation-one/) e com participação da instrutorora [Kamila Santos](https://github.com/Kamilahsantos) e demais profissionais envolvidos, tivemos a oportunidade de aprender a desenvolver um sistema de gerenciamento de Herois com as seguintes stacks abaixo.

## Stack utilizada

  * Java8
  * spring webflux
  * Spring data
  * dynamodb
  * junit
  * sl4j
  * reactor

## Executar DynamoDB Local: 

Nota: Necessário já ter uma conta na AWS - Amazon Web Services

-AWS CLI instalação: 
* https://docs.aws.amazon.com/pt_br/cli/latest/userguide/getting-started-install.html

-Gerar ID de chave de acesso e Chave de acesso secreta:
* https://docs.aws.amazon.com/pt_br/cli/latest/userguide/cli-configure-quickstart.html#cli-configure-quickstart

-Criar um usuário do IAM de administração:
* https://docs.aws.amazon.com/pt_br/mediapackage/latest/ug/setting-up-create-iam-user.html

-Navegue no terminal até a pasta em que o jar está baixado e execute: 
> $ java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb

-De posse das suas chaves de acesso, configure suas credenciais com o seguinte comando abaixo:
```shell script
$ aws configure
  << exemplo para ilustração >>
  AWS Access Key ID [None]: "digite aqui a chave gerada"
  AWS Secret Access Key [None]: "digite aqui a secret key gerada"
  Default region name [None]: sa-east-1
  Default output format [None]: json
```
-Para listar as tabelas criadas:  
> $ aws dynamodb list-tables --endpoint-url http://localhost:8000

<br>

## Documentação
Documentação gerada pela aplicação swagger: 
* http://localhost:8080/swagger-ui-heroes-reactive-api.html
