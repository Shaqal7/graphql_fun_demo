https://www.youtube.com/watch?v=kSlJH3hrV58&

Usage:
http://localhost:3000/graphiql

{
  users {
    id,
    name,
    email,
    postsCount
  }
}


mutation{
  createUser(input:{
    name: "User",
    email:"user@example.com"
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