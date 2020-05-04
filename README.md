# Docker Laravel

GitHub - https://github.com/thiagobrown/docker-laravel<br>
dockerhub - https://hub.docker.com/r/thiagobrown/laravel-app

Ambiente Laravel com:

* Laravel Framework 5.8.38
* MySQL 5.7
* Nginx 1.17.9
* PHP-FPM 7.4.5
* Redis 6.0.1

## Início

Instruções para usar o container 

### Pré-Requisitos

Para executar este container, você precisará do Docker instalado.

* **Windows** - https://docs.docker.com/windows/started/
* **OS X** - https://docs.docker.com/mac/started/
* **Linux** - https://docs.docker.com/linux/started/

### Execução

```shell
docker run -d --name <NAME> -p 8000:8000 thiagobrown/laravel-app
```

#### Variáveis de Ambiente

* `DB_HOST` - Host do banco de dados MySQL para framework Laravel
* `DB_PORT` - Port do banco de dados MySQL para framework Laravel 
* `DB_DATABASE` - Port do banco de dados MySQL para framework Laravel 
* `DB_USERNAME` - Port do banco de dados MySQL para framework Laravel 
* `DB_PASSWORD` - Port do banco de dados MySQL para framework Laravel 
* `REDIS_HOST` - Host do banco NoSQL Redis para framework Laravel 
* `APP_HOST` - Host do PHP-FPM usado Nginx
* `APP_PORT` - Port do PHP-FPM usado Nginx

## Author

**Thiago** - *Sofware Developer* - https://github.com/thiagobrown

## License

MIT License - veja em [LICENSE](LICENSE) para mais detalhes.
