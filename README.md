# docker-yeoman

Docker image with yeoman and angularjs generator installed.

### Usage

#### Grunt configuration

Find this snippet in your Gruntfile:
```
    connect: {
      options: {
        port: 9000,
        // Change this to '0.0.0.0' to access the server from outside.
        hostname: 'localhost',
        livereload: 35729
      },
```
... and change 'localhost' to '0.0.0.0'

Run it:

```
docker run -it -p 9000:9000 -p 35729:35729 --rm -v $(pwd):/src [your-image-tag] grunt serve
```
