# Q-CTRL Back-end Challenge

The Q-CTRL Back-end Challenge is a way for applicants to roles within the Q-CTRL Back-end Engineering team to demonstrate their skills and overall approach to solving a challenge based upon a set of requirements.

The requirements are intentionally sparse (the devil is in the details). We don't want you to do a lot, but what you do should be your best work and should clearly demonstrate you embody [the three virtues](https://thethreevirtues.com/).

## The Rules

- Read and understand [the challenge](#the-challenge).
- Create a solution that satisfies [the requirements](#the-requirements).
- Send a link to the repository containing your solution to the person who contacted you.

**IMPORTANT:** The repository containing your solution must be public, must contain a `README.md` file, **MUST NOT** be a fork of this repository, and **MUST NOT** make any reference to "Q-CTRL" in the repository name, description, or code.

**Note:** You should spend no more than three hours on this challenge.

## The Challenge

At Q-CTRL, we use a suite of microservices to support our products. Typically, these microservices are written using a Python web framework and expose a [GraphQL](https://graphql.org/) API so clients and other services can communicate with them.

## The requirements

- Create a new service using your Python web framework of choice (e.g. [Django](https://www.djangoproject.com/), [Flask](https://palletsprojects.com/p/flask/), [FastAPI](https://fastapi.tiangolo.com/), etc.).
- All dependencies should be captured in a `requirements.txt` file in the root of the repository.
- The service should expose a GraphQL endpoint at `/graphql`.
- The GraphQL schema should consist of a single query, `people`, which must return a list of `Person` objects.
- The `Person` object should have the following fields:
  - `email` (string).
  - `name` (string).
  - `address` (Address).
- The `Address` object should have the following fields:
  - `number` (integer).
  - `street` (string).
  - `city` (string).
  - `state` (GraphQL enum).

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

See [LICENSE](https://github.com/qctrl/back-end-challenge/blob/master/LICENSE).
