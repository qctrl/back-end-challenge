# Q-CTRL Back-end Challenge

The Q-CTRL Back-end Challenge is a way for applicants to roles within the Q-CTRL Back-end Engineering team, to demonstrate their skills and overall approach to back-end application development.

The requirements are intentionally sparse to allow some flexibility. We don't want you to do a lot, but what you do should be your best work.

## Table of Contents

  - [The Rules](#the-rules)
  - [The Challenge](#the-challenge)
  - [Contributing](#contributing)
  - [Credits](#credits)
  - [License](#license)

## The Rules

- Read and understand [The Challenge](#the-challenge).
- Create a solution that satisfies the [Requirements](#requirements).
- Send the link to the repository containing your solution to the person who contacted you.

## The Challenge

### Background

At Q-CTRL, we use a suite of microservices to support our products. Typically, these microservices are written using a Python web framework and expose a [GraphQL](https://graphql.org/) API so clients and other services can communicate with them.

### Requirements

1. Create a new GitHub repository under your account which will contain your solution. The new repository which you are going to create, should **not** be a fork of this repository and should **not** make any reference to "Q-CTRL" in the repository name, description, or code.
1. In your new repository, create a new service using the Python web framework of your choice (e.g. [Django](https://www.djangoproject.com/), [Flask](https://palletsprojects.com/p/flask/), [FastAPI](https://fastapi.tiangolo.com/), etc.).
1. All dependencies should be captured in a `requirements.txt` file at the root of the repository.
1. The service should expose a GraphQL endpoint at `/graphql`.
1. The GraphQL schema should consist of a single query, `people`, which must return a list of `Person` objects.
   - A `Person` object should have the following fields: `email` (string), `name` (string), `address` (Address).
   - An `Address` object should have the following fields: `number` (integer), `street` (string), `city` (string), `state` (GraphQL enum).

**Note:** You can choose to return your own details or use mock values.

### Validation

The following query will be used to validate your implementation:
```
query {
  people {
    email
    name
    address {
      number
      street
      city
      state
    }
  }
}
```

## Contributing

See [Contributing](https://code.q-ctrl.com/contributing).

## Credits

See [Contributors](https://github.com/qctrl/back-end-challenge/graphs/contributors).

## License

See [LICENSE](LICENSE).
