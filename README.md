# Elastic Beanstalk Docker Config Transform

This script transforms Docker configuration from Docker 1.7 and newer
`~/.docker/config.json` format to Docker 1.6 and older `~/.dockercfg` format,
as well as validates sanity of the configuration file.

If the configuration file is already in the Docker 1.6 format,
`eb-docker-config-transform` just performs validation and outputs the
file unchanged.

AWS documentation reference:
http://docs.aws.amazon.com/elasticbeanstalk/latest/dg/create_deploy_docker.html#docker-images-private

## Usage

    eb-docker-config-transform ~/.docker/config.json
    
    eb-docker-config-transform < ~/.docker/config.json

    eb-docker-config-transform ~/.dockercfg

    eb-docker-config-transform < ~/.dockercfg

## License

Released under the MIT license.
