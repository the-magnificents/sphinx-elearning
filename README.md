# Sphinx for E-learning
An example of how Sphinx can be used in online education when the participation of multidisciplinary teaching staff is required.

The repo provides a template with the bare minimum for generating documentation using Sphinx 4.x. It includes a style guide used in an online course.


--------------
## Use Case

For many years, the courseware has been prepared by at least 30 lectures with expertise in a variety of topics. A significant component of the course is the developing of practical skill for the manipulation and analysis of geographic data. Lectures prepare and update exercises for the course. A single lecturer sometimes updates exercises, but most of the times a single exercise is updated by two or more lecturers. For the sake of quality control, exercises should be revised and updated (if required) every year.

The current workflow for updating exercises relies on sharing folders thru the local network. A disadvantage of this is that when a lecturer is editing a file, no other lecturer has access to it. Therefore, they should take turns on updating each exercise. Currently, the exercises for the whole course are split into several MS Word documents. Every year, a copy of the exercises is created and placed in a new shared folder, before the process of reviewing and updating the documents can begin.

During the course, exercises are uploaded to a Learning Management System (LMS), where students will find them. Exercises are upload to the LMS as PDF files. When the exercises required urgent changes during the course, a lecturer should update the MS Word document, convert it to a PDF file, delete the current file in the LMS, upload the new file to the LMS and publishing the file to course's main page. This workflow is prone to errors, lecturers accidentally delete essential files in the LMS or upload the wrong files; after all, they have to deal with many versions and copies in the shared folders.
 
+ **Wouldn't be great if lecturers could update exercises collaboratively?** 
+ **Wouldn't be awesome if they could automate the process of updating and publishing exercises on the LMS?**
+ **In what other ways could lecturers benefit from the points above?**

-------------------------------

## Installation:

### Prerequisites:

* Python 3.6+, we tested the code using Phyton 3.8
* An IDE with support for RST. We recommend [VS Code](https://code.visualstudio.com/download)


1. Clone the repository

``` shell
git clone https://github.com/manuGil/sphinx-itc-template.git
```

2. Install Python's virtual environment


``` shell
$ apt-get install python3-venv
```

3. Go to the root of the repository and create a virtual environment

``` shell
$ cd .../sphinx-itc-template
$ python3 -m venv ./venv
```

4. Activate the virtual environment

* Linux:

``` shell
$ source ./venv/bin/activate
```

* Windows:

```shell
> .\venv\Scripts\activate
```

5. Use pip to install the required packages

``` shell
$ pip install -r requirements.txt
```

6. Go to `./docs` and compile

``` shell
$ make html
```

For more on creating your own Sphinx projects visit the [official documentation.](https://docs.readthedocs.io/en/stable/intro/getting-started-with-sphinx.html)


