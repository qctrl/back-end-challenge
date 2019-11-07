# Q-CTRL Back-end Engineering Challenge

The Q-CTRL Back-end Engineering Challenge is a way for applicants to roles within the Q-CTRL Back-end Engineering team to demonstrate their skills and overall approach to back-end application development.

## Table of Contents

- [The Rules](#the-rules)
- [The Challenge](#the-challenge)
- [Contributing](#contributing)
- [Credits](#credits)
- [License](#license)

## The Rules

- Read and understand [The Challenge](#the-challenge)
- Create a solution that satisfies the [Requirements](#requirements)
- Spend no more than two hours of actual coding time
- Send the link to the repository containing your solution to careers@q-ctrl.com

## The Challenge

### Background

There's a new set of product features being planned for [BLACK OPAL](https://q-ctrl.com/products/black-opal/) whereby a customer will be able to create and manage quantum controls. You can think of these controls as being the individual inputs a customer may employ to manipulate their quantum system using the [Q-CTRL App](https://app.q-ctrl.com/).

### Requirements

Create a web API using [Django](https://www.djangoproject.com/). The API should be backed by a [PostgreSQL](https://www.postgresql.org/) database, conform to the [JSON:API](https://jsonapi.org/) specification and should implement seven (7) API endpoints that provide the following functionality:

- Create a new control
- List all controls (five per page)
- Get a specific control
- Update a specific control
- Delete a specific control
- Bulk upload controls in CSV format
- Download controls in CSV format

### Additional Information

Below are the attributes of a control. All attributes are required.

| Name              | Description                                                                                                                     |
|-------------------|---------------------------------------------------------------------------------------------------------------------------------|
| Name              | The name of the control (e.g. "Single-Qubit Driven").                                                                           |
| Type              | Valid control types are Primitive, CORPSE, Gaussian, CinBB and CinSK.                                                           |
| Maximum Rabi Rate | The maximum achievable angular frequency of the Rabi cycle for a driven quantum transition. This is a number between 0 and 100. |
| Polar Angle       | An angle measured from the z-axis on the Bloch sphere. This is a number between 0 and 1 (units of pi).                          |

The below assets have been provided to help complete the challenge.

| Name                                | Description     |
|-------------------------------------|-----------------|
| [controls.csv](assets/controls.csv) | Sample CSV file |

## Contributing

See [Contributing](https://github.com/qctrl/.github/blob/master/CONTRIBUTING.md).

## Credits

See [Contributors](https://github.com/qctrl/back-end-challenge/graphs/contributors).

## License

See [LICENSE](LICENSE).
