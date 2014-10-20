This is a first try at defining what workflows we need and how they should look like.

## Setup Automated Build

### Initiated by

User


### Inputs 

- Repository URL
- repository credentials (?) 
- target docker registry
- docker registry credentials

### Outputs

- Git commit hook target url


## Triggered Build

### Initiated by

Git commit

### Output

- DOcker image pushed to specified registry
