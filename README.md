# Image Manipulation Rest API

## 💻 Pré-requisitos
Antes de começar, verifique se você atendeu aos seguintes requisitos:
* Você instalou a versão 7.4 de `PHP`
## 🚀 Instalando o projeto

1. Para instalar o Image Manipulation Rest API, dentro da pasta root do projeto, execute:
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

Method | endpoints | Usage
------------ | ------------- | -------------
GET | `/api/v1/album` | Lista todos os álbuns.
POST| `/api/v1/album` | Cria um novo álbum. Chave {nome}.
PUT | `/api/v1/album/` | Atualiza o {nome} de um álbum.
DELETE | `/api/v1/album` | Deleta um álbum.
GET| `/api/v1/image` | Lista todas as imagens.
GET | `/api/v1/image/{image}` | Mostra uma imagem específica.
GET | `/api/v1/image/by-album/{album}` | Mostra as imagens de álbum.
POST | `/api/v1/image/resize?w=50%` | Faz o envio de uma imagem com redimensionamento em porcentagem %.
POST | `/api/v1/image/resize?w=1024&h=1024` | Faz o envio de uma imagem com redimensionamento em pixels.
DELETE | `/api/v1/image/{image}` | Deleta uma imagem.

