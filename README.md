# Versões
debian:buster-slim

php 7.4.7

apache 2.4

laravel 7.15.0

composer 1.10.7

mysql 8.0.20

Mongo DB 4.2.8

Mongo Express 0.54.0

RabbitMQ 3.8.5

# Comandos
docker-compose up -d

# Laravel
cd application

cp .env.example .env

php artisan key:generate

# Acessar App (vhost)
http://app.local

# Configuração de Vhost Local
127.0.0.1	app.local

# Acessar Mongo Express
http://localhost:8081

usuário = root

senha = example

# Ativar Plugin RabbitMQ Management
acessar container: winpty docker exec -it rabbitmq bash

rodar comando: rabbitmq-plugins enable rabbitmq_management

obs: winpty é usado somente no windows.

# Acessar RabbitMQ Management
http://localhost:15672

usuário = guest

senha = guest