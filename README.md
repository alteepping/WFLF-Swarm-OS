## Usage
Import of builder image
oc import-image my-redhat-openjdk-18/openjdk18-openshift --from=registry.access.redhat.com/redhat-openjdk-18/openjdk18-openshift --confirm

### Template creation
oc create -f https://raw.githubusercontent.com/alteepping/WFLF-Swarm-OS/master/wildflyswarm-microservice-template.json

### Create a new App
oc new-app --template=wildflyswarm-microservice --param=APPLICATION_NAME=theNameOfTheApplication --param=REPOSITORY_URI=https://theRepositoryOfTheApplicationsSour.ce


##Additional parameters
###APPLICATION_DOMAIN
Hostname of the route to application.

###APPLICATION_PATH
Prefix of path to main rest-endpoint
