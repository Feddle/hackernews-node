# hackernews-node
GraphQL-Node hackernews clone from www.howtographql.com

Create prisma.yml:
```
endpoint: ""
datamodel: datamodel.prisma
generate:
  - generator: javascript-client
    output: ../src/generated/prisma-client
hooks:
  post-deploy:
    - prisma generate
```

run:
```
prisma deploy
```

now you can run the backend:

```
node src/index.js
```
