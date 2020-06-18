# Primeiro desafio do GoStack utilizando Node.js

### O desafio consistia em aplicar os métodos http _(POST, GET, PUT e DELETE)_ , em uma aplicação onde seria possível criar repositórios e realizar a ação de dar like. 

```javascript
    app.post("/repositories", (request, response) => {
    const { title, url, techs } = request.body;

    const repository = {
        id: uuid(),
        title,
        url,
        techs,
        likes: 0
    }
  
    repositories.push(repository);

    return response.json(repository);
```
