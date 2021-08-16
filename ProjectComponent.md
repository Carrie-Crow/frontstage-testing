# Project/Component

## Backstage Structure
https://backstage.io/docs/features/software-catalog/descriptor-format#kind-component

Relevent Fields:
```
apiVersion: backstage.io/v1alpha1
kind: Component
metadata:
    name: project-name
    description: Software that achieves goals
    links: Confluence/Cerebro link
spec:
    type: 
    lifecycle: 
    owner: deploy
    system: optional parent
```

## Cerebro Structure
Projects object relevant fields:
```
name
nickname (optional)
permalink
description (optional)
release_state_id, default: 0
category_id, default 0

```

Cerebro has a separate table to determine ownership with project_stakeholders.

## Field Mapping

| Backstage             | Cerebro                           |
| ---------             | --------                          |
| spec.type             | ?                                 |
| spec.lifecycle        | Project.release_state_id          | 
| spec.owner            | ?                                 |
| metadata.name         | Project.name? Project.nickname?   |
| metadata.description  | Project.description               |
| metadata.links        | Project.permalink                 |

## Autofill
apiVersion: backstage.io/v1alpha1
kind: Component
