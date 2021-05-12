# Symfony Framework with the MicroKernelTrait

This code runs a framework based on the MicroKernelTrait. The article was published within the web documentation:

[Building your own Framework with the MicroKernelTrait](https://symfony.com/doc/current/configuration/micro_kernel_trait.html)

## Installation

In your terminal write this command to deploy the VM.
```sh
docker-compose up --build -d
```

Docker will build the enviroments for Nginx and PHP.

Once the Docker servers have been deployed, you must access the PHP server to run composer.

```sh
docker exec -it php8.0.6 bash
```

In the /var/www folder run composer to start downloading the vendor files.
```sh
composer update
composer install
```

Verify the deployment by navigating to your server address in your preferred browser.

```sh
127.0.0.1:5000
localhost:5000
http://127.0.0.1:5000/random/10
```
## Docker

- PHP 8.0.6
- Nginx 1.6

## Development

- Define routes, services, and configurations by YAML files.
