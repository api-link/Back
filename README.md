
<p align="center">
  <a href="https://www.aichner-christian.com/" target="_blank" rel="noopener noreferrer">
    <img src="https://www.aichner-christian.com/img/logo/apilink.png" alt="Api Link Logo" height="150">
  </a>
</p>

<h3 align="center">API Link - Connect your sources</h3>

<p align="center">
  API Link is a service built to make APIs more accessible and usable by taking away all your pain of setting up multiple APIs connectors. We handle all your required APIs and deliver one single beautiful stream of data.
  <br>
  <br>  
  <a href="https://github.com/api-link/Back/issues/new?template=bug_report.md">Report bug</a>
  ·
  <a href="https://github.com/api-link/Back/issues/new?template=feature_request.md">Request feature</a>  ·
  <a href="https://github.com/api-link/Back/issues/new?template=change_request.md">Request change</a>
</p>

## Table of contents

- [Quick start](#quick-start)
- [Bugs and feature requests](#bugs-and-feature-requests)
- [Contributing](#contributing)
- [Versioning](#versioning)
- [Creators](#creators)
- [Thanks](#thanks)
- [Copyright and license](#copyright-and-license)

## [](#quick-start)Quick start
Choose setup for:
- [Docker](#setup-with-docker)
- [Python Virtual Environment](#setup-with-python-virtual-environment)

## [](#setup-with-docker)Setup with Docker

#### Dependencies

- [Docker](https://docs.docker.com/engine/installation/)
- [Docker Compose](https://docs.docker.com/compose/install/)

### Installation

Run the following commands:

```bash
git clone https://github.com/api-link/Back.git api-link-django
cd api-link-django
docker-compose up --build -d
docker-compose up
```

The demo site will now be accessible at [http://localhost:8000/](http://localhost:8000/).

**Important:** This `docker-compose.yml` is configured for local testing only, and is _not_ intended for production use.

### Debugging

To tail the logs from the Docker containers in realtime, run:

```bash
docker-compose logs -f
```

## [](#setup-with-python-virtual-environment)Setup with Python Virtual Environment

You can run this Django application without setting up Docker and simply use a virtual environment,
which is the [recommended installation approach](https://docs.python.org/3/library/venv.html) for all Python projects itself.

#### Dependencies

- Python 3.5, 3.6 or 3.7

### Installation

With [PIP](https://github.com/pypa/pip) installed, run:

    git clone https://github.com/api-link/Back.git api-link-django
    cd api-link-django
    python --version
    python -m pip --version

Confirm that this is showing a compatible version of Python 3.x. If not, and you have multiple versions
of Python installed on your system, you may need to specify the appropriate version when creating the venv:

    python3 -m venv /path/to/new/virtual/environment

Once a virtual environment has been created, it can be “activated” using a script in the virtual environment’s
binary directory. The invocation of the script is platform-specific (<venv> must be replaced by the path of the
directory containing the virtual environment):

| Platform | Shell      | Command to activate virtual environment |
| :------- | :--------- | :-------------------------------------- |
| Posix    | bash/zsh   | \$ source <venv>/bin/activate           |
|          | fish       | \$ . <venv>/bin/activate.fish           |
|          | csh/tcsh   | \$ source <venv>/bin/activate.csh       |
| Windows  | cmd.exe    | C:\> <venv>\Scripts\activate.bat        |
|          | PowerShell | PS C:\> <venv>\Scripts\Activate.ps1     |

Now we're ready to set up the project itself:

    pip install -r requirements/base.txt

To set up your database and load initial data, run the following commands:

    ./manage.py migrate
    ./manage.py runserver

## [](#bug-and-feature-requests)Bugs and feature requests

Have a bug or a feature request? Please first search for existing and closed issues. If your problem or idea is not
addressed yet, [please open a new issue](https://github.com/api-link/Back/issues/new/choose).

## [](#contributing)Contributing

![GitHub last commit](https://img.shields.io/github/last-commit/api-link/Back)
![GitHub issues](https://img.shields.io/github/issues-raw/api-link/Back)
![GitHub closed issues](https://img.shields.io/github/issues-closed-raw/api-link/Back?color=green)

Please read through our [contributing guidelines](https://github.com/api-link/Back/blob/master/CONTRIBUTING.md).
Included are directions for opening issues, coding standards, and notes on development.

All HTML and CSS should conform to the [Code Guide](https://github.com/mdo/code-guide), maintained by [Mark Otto](https://github.com/mdo).

## [](#versioning)Versioning

For transparency into our release cycle and in striving to maintain backward compatibility, this repository is
maintained under [the Semantic Versioning guidelines](https://semver.org/). Sometimes we screw up, but we adhere to
those rules whenever possible.

## [](#creators)Creators

**Simon Prast**

- <https://github.com/dermrsimon>
- <https://www.linkedin.com/in/simonprast/>

**Christian Aichner**

- <https://twitter.com/realaichner>
- <https://www.facebook.com/aichner.christian>
- <https://github.com/Aichnerc>

**Florian Kleber**

- <https://github.com/kleberbaum>

## [](#thanks)Thanks

We do not have any external contributors yet, but if you want your name to be here, feel free
to [contribute to our project](#contributing).

## [](#copyright-and-license)Copyright and license

![GitHub repository license](https://img.shields.io/badge/license-EUPL--1.2-blue)

SPDX-License-Identifier: (EUPL-1.2)
Copyright © 2019 Werbeagentur Christian Aichner