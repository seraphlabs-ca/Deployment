# Deployment

A collection of scripts to deploy different packages on different platforms.

## Usage

The deployment process is controlled by environment variables. Make sure to configure ```s3cmd``` with the right permissions to match the S3 bucket. The bucket structure is assumed to be the same as ```Deployment```, that is: ```<package>/<platform>/[DATA FILES].

### Configuration

```
export DEPLOYMENT_S3_BUCKET=<Your deployment bucket>
```

### Package Deployment

Execute the following command in order to deploy package ```<package>``` under platform ```<platform>```.
```
./packages/<package name>/<platform>/deploy
```
