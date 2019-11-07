# Q-CTRL Back-end Engineering Challenge

The Q-CTRL Back-end Engineering Challenge is a way for applicants to roles within the Q-CTRL Back-end Engineering team to demonstrate their skills and overall approach to back-end web application development.

## Table of Contents

- [The Rules](#the-rules)
- [The Challenge](#the-challenge)
- [Contributing](#contributing)
- [Credits](#credits)
- [License](#license)

## The Rules

- Read and understand [The Challenge](#the-challenge)
- Create a [Django](https://www.djangoproject.com/) app that satisfies the [Requirements](#requirements)
- Spend no more than one hour of actual coding time
- Send the link to the repository containing your app to careers@q-ctrl.com

## The Challenge

### Background

There's a new set of product features being planned for [BLACK OPAL](https://q-ctrl.com/products/black-opal/) whereby a customer will be able to create and manage quantum controls. You can think of these controls as being the individual inputs a customer may employ to manipulate their quantum system using the [Q-CTRL App](https://app.q-ctrl.com/). The customer will be able to:

- Create a new control
- View a list of controls (five per page)
- View the details of a control
- Update the details of a control
- Delete a control
- Bulk upload controls in CSV format
- Download controls in CSV format

### Requirements

#### Manage Controls

Implement API endpoints that can:

- Create a new control
- List all controls (five per page)
- Get a specific control
- Update a specific control
- Delete a specific control

#### Upload Controls

Implement an endpoint that can accept a CSV file where each row represents a control (see the Additional Information section below for an example CSV file).

#### Download Controls

Implement an endpoint that returns all controls in CSV format. (see the Additional Information section below for a sample CSV file).

### Additional Information

Below are the attributes of a control. All attributes are required.

| Name              | Description                                                                                                                     |
|-------------------|---------------------------------------------------------------------------------------------------------------------------------|
| Name              | The name of the control (e.g. "Single-Qubit Driven").                                                                           |
| Type              | Valid control types are Primitive, CORPSE, Gaussian, CinBB and CinSK.                                                           |
| Maximum Rabi Rate | The maximum achievable angular frequency of the Rabi cycle for a driven quantum transition. This is a number between 0 and 100. |
| Polar Angle       | An angle measured from the z-axis on the Bloch sphere. This is a number between 0 and 1 (units of pi).                          |

### Assets

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
