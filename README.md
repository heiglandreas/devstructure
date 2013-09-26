#DevStructure

This package will create a development structure and install all tools
necessarry for easy development

During installation this package will create a complete folderstructure so that
you can start coding right away.

The structure contains the following:

* **build** - contains all your build artifacts
* **src**   - contains the sourcecode of your project
* **doc**   - contains the documentation of your project
* **doc/api** - contains the output of phpDocumentor
* **doc/coverage** - contains the code-coverage-report
* **vendor** - contains all the additional libraries that you imported
* **dist**  - contains the distribution-files of your project
* **tests** - containing your test-files

##Installation

### Create your ' soon to be a project'-folder

```bash
mkdir MyNewProjectFolder
````

### Move into your newly created project folder

```bash
cd MyNewProjectFolder
````

### Create a ```composer.json```-file in your newly created project-folder

Either install it by cloning the example-file into your project-folder

```bash
curl -o composer.json https://raw.github.com/heiglandreas/devstructure/master/example.composer.json
# OR
wget https://raw.github.com/heiglandreas/devstructure/master/example.composer.json > composer.json
```

Or you create the file with your favourite text-editor. Insert at least the following content

```JSON
{
    "require-dev" : {
        "org_heigl/devpackages" : "dev-master"
    },
    "minimum-stability": "dev",
    "config" : {
        "bin-dir" : "bin"
    }
}
```

You can use the file ```example.composer.json``` as template.

### Install ```composer``` 

```bash
curl -sS https://getcomposer.org/installer | php
````

### Run composer

```bash
php composer.phar install
````

### Use your complete development infrastructure

Including all of the above tools including cool phing tasks that make your live easier

