# Todos API

## What is this?

This is an API that uses jwt web tokens in order to release data on the command line.

## Development

### Setup 

* git clone application
* bundle install
* brew install httpie

### Run

```bash
# user signup
$ http POST :3000/auth/signup Accept:'application/vnd.todos.2+json' email=user@test.co.uk password=password password_confirmation=password
# copy authorization key
# Post a todo
$ http POST :3000/todos title="Go swimming" Authorization='NUMBER ABOVE'
# Access todo
$ http :3000/todos Accept:"application/vnd.todos.v1+json" Authorization:'NUMBER ABOVE'
```

