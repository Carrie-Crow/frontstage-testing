# Repository Purpose
This repo is for creating a Github location for a Backstage yaml configuration file to redirect too for the Zendesk/Frontstage repo.

# Backstage YAML Entities
These are the types of objects necessary to create a functioning backstage.

## Initial Entities
The relevant entities for the Deploy Productivity proof of concept.

### Project/Component
https://backstage.io/docs/features/software-catalog/descriptor-format#kind-component
See Project/Component.md for the mapping of the Backstage Components to Cerebro Projects.

### Teams/Group
https://backstage.io/docs/features/software-catalog/descriptor-format#kind-group
See TeamsGroup.md for the mapping of the Backstage Groups to Cerebro Teams.

### User
https://backstage.io/docs/features/software-catalog/descriptor-format#kind-user
See Users.md for the mapping of the Backstage User to Cerebro Users.
apiVersion
kind

spec
    * memberOf

metadata
    * name
    * description
    * links


## Maybe Needed
### Resource
https://backstage.io/docs/features/software-catalog/descriptor-format#kind-resource

apiVersion
kind

spec
    * owner
    * type
    * system (optional)

metadata
    * name
    * description
    * links

### Location
https://backstage.io/docs/features/software-catalog/descriptor-format#kind-location

apiVersion
kind

metadata
    * name
    * description
    * links


### System
https://backstage.io/docs/features/software-catalog/descriptor-format#kind-system


apiVersion
kind 

metadata
    * name
    * description
    * links