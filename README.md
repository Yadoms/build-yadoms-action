# build-yadoms-action github action

This action allow to generate a yadoms build using Github Actions.

## Inputs

### `who-to-greet`

**Required** The name of the person to greet. Default `"World"`.


### `privileged`

* optional * To run the container in privileged mode, set this input to "--privileged"


### `entrypoint`

* optional * The entrypoint override (default : /entrypoint.sh)

### `param1`, `param2`, `param3`, `param4`

* optional * Free parameters passed to docker container

## Outputs

### `yadomsVersion`

The current building yadoms full version, example : '2.5.0-beta.1'


## Example usage

- name: Yadoms build script
  uses: Yadoms/build-yadoms-action@v3.beta3
  