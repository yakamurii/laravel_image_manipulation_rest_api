# Image Manipulation Rest API

## 💻 Pré-requisitos
Antes de começar, verifique se você atendeu aos seguintes requisitos:
* Você instalou a versão 7.4 de `PHP`
## 🚀 Instalando o projeto

1. Para instalar o Image Manipulation Rest API, siga estas etapas:

Dentro da pasta root do projeto, execute:
```
composer install
```
2. Copie o conteúdo de  `.env.example` para  `.env`.
3. Faça os ajustes para o banco de dados que preferir.
4. Dentro da pasta root do projeto, execute:
```
php artisan key:generate --ansi
```
5. Dentro da pasta root do projeto, execute:
```
php artisan migrate
```
6. Dentro da pasta root do projeto, execute:
```
php artisan serve
```
## Como usar 

Método | endpoint
------------ | -------------
GET | `http://127.0.0.1:8000/api/v1/album`
POST| `http://127.0.0.1:8000/api/v1/album`
PUT | `http://127.0.0.1:8000/api/v1/album`
DELETE | `http://127.0.0.1:8000/api/v1/album`
GET| `http://127.0.0.1:8000/api/v1/image`
GET | `http://127.0.0.1:8000/api/v1/image/{image}`
GET | `http://127.0.0.1:8000/api/v1/image/by-album/{album}`
POST | `http://127.0.0.1:8000/api/v1/image/resize?w=50%`
POST | `http://127.0.0.1:8000/api/v1/image/resize?w=1024&h=1024`
DELETE | `http://127.0.0.1:8000/api/v1/image/{image}`

