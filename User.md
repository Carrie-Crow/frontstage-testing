# User
## Backstage Structure
https://backstage.io/docs/features/software-catalog/descriptor-format#kind-user

Relevent Fields:
```
apiVersion: backstage.io/v1alpha1
kind: User
metadata:
    name: carrie.crow
    links: URL?
spec:
    memberOf: deploy
    profile:
        email: Carrie.Crow@zendesk.com
```

## Cerebro Structure
User object relevant fields:
```
name
permalink
email
admin (boolean)

```

Cerebro assigns user objects to the Team object

## Field Mapping

| Backstage             | Cerebro           |
| ---------             | --------          |
| spec.memberOf         | ?                 |
| spec.profile.email    | User.email        | 
| metadata.name         | User.name         |
| metadata.links        | User.permalink    |

## Autofill
apiVersion: backstage.io/v1alpha1
kind: Component
