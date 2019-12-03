# How To Use GraphQL with Ruby on Rails

[Link to YT HowTo](https://www.youtube.com/watch?v=kSlJH3hrV58&)

### Usages

On Rails APP

[http://localhost:3000/graphiql](http://localhost:3000/graphiql)

#### QUERY　

```json
{
	users {
		id,
		name,
		email,
		postsCount
	}
}
```
#### MUTATIONS　
```json
mutation {
	createUser(
		input: {
			name: "User",
			email: "user@example.com"
		}) {
		user{
			id,
			name,
			email
			posts {
				title
			}
		}
		errors
	}
}
```

Frontend is used React.

### How use:

In project folder use:

rails s

In folder 'frontend' use:

yarn start

In terminal can ask you about port 3000 cause it's already use, so say Y(yes) for other port, and it will be use on 3001


Go to web browser on localhost:3001