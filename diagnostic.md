# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
We like to have a backend if we want to be able to save things/hold data since the browser doesn't really hold that kind of info for us... Basically once an application gets to the client, it's completely separated from everything else unless we have a backend.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
The model
```

Which layer in the MVC pattern communicates with the model?

```md
The controller
```

Why don't we use views in our interpretation of the MVC pattern?

```md
It's just stuff/data that gets sent back to the client... it's more for the user than the developer. We replace views with serializers in Rails.
```

What does C.R.U.D stand for?

```md
Create
Read
Update
Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
The controller
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
create
index
show
update
destroy
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
The client sends the request GET /people/1 to the API
The router points the request to the controller
The controller asks the model to get the information
The model looks at the database and sends it back to the controller
The controller makes the information easier to read for the client
The controller then sends that information back ot the client
```

What is the command to generate a new rails-api app?

```bash
bin/rake [db:drop] db:create db:migrate db:seed db:examples
```

What is the command to start an instance of a rails server?

```bash
bin/rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
- bin/rake db:drop
- bin/rake db:create
- bin/rake db:migrate
- bin/rake db:seed
- bin/rake db:examples
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bin/rails generate scaffold pet name:text age:integer
```
