# Background

This exercise is a learning exercise for SMART on FHIR, using a publicly available SMART on FHIR endpoint. Note that a user account exists with credentials username = `test` and password = `test`.

# Starting a Server in this directory

In order to serve the files in this directory as HTTP, you need an HTTP sever that can serve a diretory. One very easy way to do this is by using Python. You may have to [install Python](https://www.python.org/downloads/) for this to work.

The following command tests whether Python is installed.

```bash
python -V
```

The following commands start a server in the current directory using port 8080.

```bash
# If Python version returned above is 3.X
python -m http.server 8080
# If Python version returned above is 2.X
python -m SimpleHTTPServer 8080
```

# Task

Try launching this app by starting the local server then navigating to http://localhost:8080/launch.html

Once you have this working:

* Grab the access token and decode it using the JWT decoder at: http://calebb.net/
* Grab the ID token and decode it using the JWT decoder at: http://calebb.net/
* Use the Access Token to read more FHIR data for the context patient

More advanced:

* Try requesting a write scope and pushing data to the server for this patient