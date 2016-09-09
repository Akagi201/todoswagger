
## Steps

```
❯ swagger init spec --title "A To Do list application" --description "The product of a tutorial on goswagger.io" --version 1.0.0 --scheme http --consumes application/io.goswagger.examples.todo-list.v1+json --produces application/io.goswagger.examples.todo-list.v1+json
2016/09/02 11:29:17 creating specification document in Users/akagi201/Documents/learning-golang/src/swagger/todo/swagger.yml
```

```
❯ swagger validate ./swagger.yml
The swagger spec at "./swagger.yml" is valid against swagger specification 2.0
```

```
edit swagger.yml
```

```
swagger generate server -A TodoList -f ./swagger.yml
```

```
swagger generate client -A TodoList -f ./swagger.yml
```

```
cd cmd/todo-list-server
go build
```
