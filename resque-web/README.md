# Resque Web Interface

## Usage:

Standard port, database 0:

```
    docker run -it --rm -p 5678:5678 -e redis=your-redis.example.com carloslima/resque-web
```

Different port:

```
    docker run -it --rm -p 5678:5678 -e redis=your-redis.example.com:9736 carloslima/resque-web
```

Different database:

```
    docker run -it --rm -p 5678:5678 -e redis=your-redis.example.com:6379:2 carloslima/resque-web
```

Access the interface at: http://localhost:5678
