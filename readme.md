
### Curl command for Curl-request-5-POST using Explicit flag (which means use -X)

-we can also use -H in place of --header
, and -d in place of --data

```js
curl -X POST --header "Content-Type: application/json" -d "{\"userId\": \"1\", \"id\":\"1\", \"title\": \"delectus aut autem\",\"completed\":\"false\"}" https://jsonplaceholder.typicode.com/todos (make a post request using the /todos endpoint, using explicit flag ( which means use -X ))
```
```js
curl -o todoPost.txt -X POST --header "Content-Type: application/json" -d "{\"userId\": \"1\", \"id\":\"1\", \"title\": \"delectus aut autem\",\"completed\":\"false\"}" https://jsonplaceholder.typicode.com/todos (to store the todos post request in todoPost.txt)
```



using a similar schema and pass required fields in your request: 
{
    "userId": 1,
    "id": 1,
    "title": "delectus aut autem",
    "completed": false
}

into curl commant below: 
```js
curl -X POST --header "Content-Type: application/json" -d "{\"userId\": \"1\", \"id\":\"1\", \"title\": \"delectus aut autem\",\"completed\":\"false\"}" https://jsonplaceholder.typicode.com/todos 
```


Post response from:
```js
curl -X POST --header "Content-Type: application/json" -d "{\"userId\": \"1\", \"id\":\"1\", \"title\": \"delectus aut autem\",\"completed\":\"false\"}" https://jsonplaceholder.typicode.com/todos 
```
{
  "userId": "1",
  "id": 201,
  "title": "delectus aut autem",
  "completed": "false"
}
