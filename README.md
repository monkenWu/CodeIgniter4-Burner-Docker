# CodeIgniter4-Burner-Docker

CodeIgniter4 Burner Recommended Docker Configuration.

## Quick Start

* Place your CodeIgniter4 project in the `app` folder.
* Build your environment with `docker-compose build`
* Use `docker-compose up -d` to make the container run in the background.
* Use `docker-compose exec app bash` to get into the container.
* By default you will be located in the root directory of your project and you can start installing Burner and selecting the Dirver you need. 

> If your CodeIgniter4 does not contain the `vendor` folder, remember to use `composer install` to pull the required libraries for your project.

## Notes

1. All recommended configurations are based on the [webdevops/Dockerfile](https://github.com/webdevops/Dockerfile) image.

2. This image has most common PHP extensions turned on by default, and you can refer to this [DOC](https://dockerfile.readthedocs.io/en/latest/content/DockerImages/dockerfiles/php.html
) to control more PHP configurations for your project.

3. The OpenSwoole Dockerfile references the [official OpenSwoole Dockerfile](https://github.com/openswoole/docker-openswoole/tree/master/dockerfiles).

4. The Workerman Dockerfile additionally installs the `php-event` extension, which allows Workerman to perform better.

