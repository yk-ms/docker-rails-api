# docker-rails-api
* Ruby on Rails 5 API mode sample on Docker

## Usage
### Build

```
$ cd /path/to/docker-rails-api
$ docker-compose -f docker-compose.development.yml build
```

### Database Creation

```
$ docker-compose -f docker-compose.development.yml run --rm web rake db:create
```

### Table Creation
```
$ docker-compose -f docker-compose.development.yml run --rm web ridgepole -c config/database.yml -E development --apply -f db/schemas/Schemafile
```

### Up

```
$ docker-compose -f docker-compose.development.yml up -d
```

### Access

```
$ open http://localhost:3000
```
