# Sphinx for E-learning
An example of how Sphinx can be used in online education when the participation of multidisciplinary teaching staff is required.

The repo provides a template with the bare minimun for generating documentation using Sphinx 4.x. It includes a style guide used in an online course.

## Use Case

For many years, the courseware has been prepared by at least 30 lectures with expertise in a variety of topics. A major component of the course is the developig of practical skill for the manipulation and analysis of geographic data. Lectures prepare and update exercises for the course, exercise are sometime updated by a single lecturer, but most of the times a single exercise is updated by two or more lecturers. For the sake of quality control, exercises should be revised and updated (if required) every year.

The current workflow for updating exercises relies on sharing folders thru the local network. A disavantange of this is that when a lecturer is editing a file, no other lecturer has access to it. Therefore, they should have turns on apdating each exercise. Currently, the exercise for the whole course are split in several MS Word documents. Every year, a copy of the exercises is created beore the process of reviewing and updating the documents begin.

During the course exercies are uploaded to a Learning Management System (LMS) where students will find them. Exercises are upload to the LMS as PDF files. When the exercises required urgent changes during the course, a lecturer should update the MS Word document, convert it to a PDF file, delete the current file in the LMS, upload the new file to the LMS and publising the file to course's main page. This workflow is prone to errors, lecturers accidentally delete important files in the LMS or upload the wrong files; after all they have deal with many versions and copies in the shared folders.
 
+ Wouldn't be grate if lecturers could update exercises collaboratively? 
+ Wouldn't be awesome if they could automate the process of updating and publishing exercises on the LMS?
+ In what other ways could lecturers benefit from the points above?


## Prerequisits:

* Python 3.6+, we tested the code using Phyton 3.8
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

For more on creating you own Sphinx projects visit the [official documentation.](https://docs.readthedocs.io/en/stable/intro/getting-started-with-sphinx.html)


