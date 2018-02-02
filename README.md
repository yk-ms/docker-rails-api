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

### Up

```
$ docker-compose -f docker-compose.development.yml up -d
```

### Access

```
$ open http://localhost:3000
```
