# docker-crowi

* [Crowi wiki](http://site.crowi.wiki/) on Docker

## Example docker-compose.yml

```yaml
crowi:
    #image: bakudankun/crowi
    image: tukiyo3/crowi
    links:
        - db
        - redis
    ports:
        - 8080:3000

db:
    image: mongo

redis:
    image: redis:alpine
```
