# Teams/Groups

## Backstage Structure
https://backstage.io/docs/features/software-catalog/descriptor-format#kind-group

Relevent Fields:
```
apiVersion: backstage.io/v1alpha1
kind: Group
metadata
    name: deploy
    description: Manages company deployments
    links: Confluence link
spec
    type: team
    members: team members
    parent: engineering
```

## Cerebro Structure
Team object relevant fields:
```
name
permalink
description (optional)
office_id (optional)
parent_id (optional)
```

## Field Mapping

| Backstage             | Cerebro           |
| ---------             | --------          |
| spec.type             | ?                 |
| spec.parent           | Team.parent_id    |
| metadata.name         | Team.name         |
| metadata.description  | Team.description  |
| metadata.links        | Teams.permalink   |

## Autofill
apiVersion: backstage.io/v1alpha1
kind: Group
spec
    type: team