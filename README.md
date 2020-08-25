# Sphinx Template
The bare minimun for generating documentation using Sphinx 4.x. It includes a style guide and a virtual environment with Python 3.8 and the required extension

## Prerequisits:

* Python 3.6+, we tested the code using Pyton 3.8
* An IDE with support for RST. We recommend [VS Code](https://code.visualstudio.com/download)

## Installation:

1. Clone the repository

``` shell
git clone https://github.com/manuGil/sphinx-itc-template.git
```

2. Go to the root of the repository and create a virtual environment

``` shell
$ cd .../sphinx-itc-template
$ python3 -m venv ./venv
```

3. Activate the virtual environment

* Linux:

``` shell
$ source ./venv/bin/activate
```

* Windows:

```shell
> .\venv\Scripts\activate
```

4. Use pip to install the required packages

``` shell
$ pip install -r requirements.txt
```

3. Go to `./docs` and compile

``` shell
$ make html
```

For more on creating you own Sphinx projects visit the [official documentation](https://docs.readthedocs.io/en/stable/intro/getting-started-with-sphinx.html)


