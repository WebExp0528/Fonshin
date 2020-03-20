### Installing

#### Manual

```bash
# Clone the project and run composer
git clone https://github.com/WebExp0528/Fonshin.git
cd fonshin

# Migration and DB seeder (after changing your DB settings in .env)
php artisan migrate --seed

# Install passport
php artisan passport:install

# Install dependency with NPM
npm install

# develop
npm run dev # or npm run watch

# Build on production
npm  run production
```

#### Docker

```sh
docker-compose up -d
```

Run database migration and seed within Docker container

```sh
# Get laravel docker container ID from containers list
docker ps

docker exec -it fonshin_laravel_1 php artisan migrate --seed
# Where <container ID> is the "laravel" container name, ex: docker_laravel_1
```

`npm` commands are also supported:

```sh
docker exec -it fonshin_laravel_1 npm run watch
# Where <container ID> is the "laravel" container name, ex: docker_laravel_1
...
```

## Running the tests

- Tests system is under development

## Deployment and/or CI/CD

coming soon

## Built with

- [Laravel](https://laravel.com/) - The PHP Framework For Web Artisans
- [VueJS](https://vuejs.org/) - The Progressive JavaScript Framework
- [Element](https://element.eleme.io/) - A Vue 2.0 based component library for developers, designers and product managers
- [Vue Admin Template](https://github.com/PanJiaChen/vue-admin-template) - A minimal vue admin template with Element UI

## Related projects

- [Laravue-core](https://github.com/tuandm/laravue-core) - Laravel package which provides core functionalities of Laravue.

## Acknowledgements

- [vue-element-admin](https://panjiachen.github.io/vue-element-admin/#/) A magical vue admin which insprited Laravue project.
- [tui.editor](https://github.com/nhnent/tui.editor) - Markdown WYSIWYG Editor.
- [Echarts](http://echarts.apache.org/) - A powerful, interactive charting and visualization library for browser.
