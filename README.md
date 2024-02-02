# Teste DevOps

## 🚀 Começando

Precisamos criar então uma Pipeline no Github Actions que faça o deploy do site no Cloud Run, por trás do Cloud Run precisamos que contenha um Load Balancer.

### 📋 Necessidades

* Subir um site em qualquer linguagem, o Docker pode ser o mais simples possível.
* O servidor HTTP deverá ser um apache2
* Quero que a porta do meu apache fique flexível, aceitando qualquer valor que eu passe no Cloud Run.(Por padrão o Cloud 
Run consegue enviar um valor para uma váriavel chamada $PORT), caso não consiga quero ele rodando na porta 300.
* A Pipeline não poderá conter nada sensível escrito diretamente nela, devemos usar secrets. No nome do projeto do GCP, imagem e etc...
* Meu servidor deverá ser hospedado no us-east1, e também que seja publica e não privada.
* Quero um Load Balancer nesse Cloud Run, e que ele use certificado e só trafegue por https.
* DNS = ideaads.com.br e www.ideaads.com.br
* quero passar meu site aqui https://www.ssllabs.com/ssltest e aqui https://securityheaders.com/ e que eles me retornem um Overall Rating A


### Observações

* Já possui um DNS cadastrado nesse projeto do gcp, usem ele.. é esse ideaads.
* Seria interessante concluir todas as tasks, mas caso não consiga, entregue o máximo que puder.
* Estamos utilizando o GCP aqui na ideamaker, portanto o teste deverá ser no GCP.
* Em caso de dúvidas ou qualquer problema, enviem um email para bruno.casarini@ideamaker.com.br e joao-gabriel@ideamaker.com.br
* Criar uma service account no gcp com somente as permissões necessárias para o envio da imagem.