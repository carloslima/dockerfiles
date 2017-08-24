# Divolte

[![](https://badge.imagelayers.io/carloslima/divolte:latest.svg)](https://imagelayers.io/?images=carloslima/divolte:latest)

## Usage:

Standard port, default configuration:

```
    docker run -it --rm -p 8290:8290 carloslima/divolte
```

Standard port, custom configuration:

```
    docker run -it --rm -p 8290:8290 -v ./divolte.conf:/opt/divolte/conf/divolte-collector.conf carloslima/divolte
```

Access the interface at: http://localhost:8290
