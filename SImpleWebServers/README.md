# Simple Web server with Golang

This repo represents a simple web server developed using the Go language.

## Route mechanism
We will have 3 end-points:
- `/` which will return the index.html
- `/hello` which will call the hello func and print "hello" to the screen.
- `/form.html` which will call the form func and return a form page


## How to build
1. First make sure to start your go package with <code>go mod init main</code><br>

2. Now build an executable with <code>go build</code>

3. Finally, run the executable with <code>go run main.go</code>

4. You can now test the application on http://localhost:8008