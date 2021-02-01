## Doctrine json type unescaped
By default json Doctrine types escape unicode characters before storing strings in the database.  
JsonUnescapedType override default JsonType to prevent this.  

#### Symfony integration
```yaml
# config/packages/doctrine.yaml
doctrine:
    dbal:
        types:
            json: Luzrain\DoctrineJsonUnescapedType\JsonUnescapedType
```
