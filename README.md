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
