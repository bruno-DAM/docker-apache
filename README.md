# docker-apache

- Atividade  - Criando um Container de uma Aplicação WEB DIO.me;

- Proposta: utilizar o docker compose para executar uma aplicação HTML em um container Apache.

### Estrutura do projeto 
```
app/
  index.html
  apache.yml
```
  

### Passos para rodar a aplicação

```
# Criação de diretório e arquivos

git clone https://github.com/bruno-DAM/docker-apache

cd docker-apache

mkdir servidor_web

cd servidor_web

nano index.html 
```

No arquivo **index.html** (no **h1** pode colocar o que quiser).

```
<html>
  <h1>Parabéns, aqui está seu primeiro servidor web!</h1>
</html>
```

Para salvar arquivo e sair do **nano**: **ctrl + O, ctrl + X**

```
# instalação do docker-compose e subindo container

apt install docker-compose

docker-compose -f apache.yml up -d

docker container ls
```

Após isso, colocar no nevagor o endereço IP do servidor.
