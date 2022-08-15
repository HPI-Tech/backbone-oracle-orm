### Start the application

```bash
# Via air (hot reload)
air

# Or go run
go run main.go serve

# down packages
go mod vendor

# VSCode debug
Just F5 😄
```

### Use docker-compose

```
# Run docker-compose (run docker-compose with specific env file)
docker-compose --env-file .env.{*your_env_file} up
```

### Generate swagger

```
# Generate api description into swagger docs
swag init -g main.go
```

## Production

```bash
docker build -t gohexaboi .
docker run -d -p 3000:3000 gohexaboi
```

Go to http://localhost:3000
