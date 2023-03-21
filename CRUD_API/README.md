# **CRUD API with Golang**

Setup a simple CRUD API to access a movie database (database is currently a simple slice in the code).

### How to build
1. Run `go mod tidy`
2. Run `go build`
3. Run `go run main.go` 

Now you have a server accessible on port 8000 at http://localhost:8000

## **Actions to perform**
You can test and send HTTP request to the above mentioned endpoint to perform several actions on the movies '_database_':

- Fetch all movies: GET http://localhost:8000/movies
- Create a new movie: POST http://localhost:8000/movies (Send in the data in JSON format withh all the appropriate fields)
- Delete a movie: DELETE http://localhost:8000/id This is the ID of the movie you wish to delete)
- Update a movie: PUT http://localhost:8000/id (This is the ID of the movie you wish to update)
- Fetch a specific movie: GET http://localhost:8000/id


Example of a JSON body (Note that on creation the ID will be automatically generate):
```
{
    "isbn": "8283278",
    "title": "Movie Seven",
    "director": {
        "firstname": "Marie Anne",
        "lastname": "Monroe"
    }
}
```