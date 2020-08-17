# build-yadoms-action github action

This action allow to generate a yadoms build using Github Actions.

## Inputs

### `who-to-greet`

**Required** The name of the person to greet. Default `"World"`.


### `privileged`

To run the container in privileged mode, set this input to "--privileged"

### `repository`

The yadoms source repository to build
Z

  repository: 
    description: 'Base repository url'
    required: false
    default: 'https://github.com/Yadoms/yadoms.git'
    
  branch: 
    description: 'Branch to build'
    required: false
    default: 'master'
    
  param1: 
    description: 'Generic parameter 1'
    required: false
    default: ''
    
  param2: 
    description: 'Generic parameter 1'
    required: false
    default: ''

  param3: 
    description: 'Generic parameter 3'
    required: false
    default: ''

  param4: 
    description: 'Generic parameter 4'
    required: false
    default: ''
        
  entrypoint: 
    description: 'entrypoint override'
    required: false
    default: '/entrypoint.sh'


## Example usage

uses: actions/hello-world-docker-action@v1
with:
  who-to-greet: 'Mona the Octocat'