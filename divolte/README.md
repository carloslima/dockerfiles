# Divolte

[![](https://badge.imagelayers.io/carloslima/divolte:latest.svg)](https://imagelayers.io/?images=carloslima/divolte:latest)

## Usage:

Standard port, default configuration:

```
    docker run -it --rm -p 8290:8290 carloslima/divolte:0.5.0
```

Standard port, custom configuration:

```
    docker run -it --rm -p 8290:8290 -v ./divolte.conf:/opt/divolte/conf/divolte-collector.conf carloslima/divolte:0.5.0
```

Access the interface at: http://localhost:8290
