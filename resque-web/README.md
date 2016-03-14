# Resque Web Interface

## Usage:

    docker run --rm -p 5678:5678 -e redis=your-redis.example.com carloslima/resque-web

    docker run --rm -p 5678:5678 -e redis=your-redis.example.com:6379 carloslima/resque-web

    docker run --rm -p 5678:5678 -e redis=your-redis.example.com:6379:0 carloslima/resque-web
