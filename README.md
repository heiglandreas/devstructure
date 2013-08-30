#DevStructure

This package will create a development structure and install all tools
necessarry for easy development

During installation this package will create a complete folderstructure so that
you can start coding right away.

The structure contains the following:

* **build** - contains all your build artifacts
* **src**   - contains the sourcecode of your project
* **doc**   - contains the documentation of your project
* **doc/api** - contains the output of pgpDocumentor
* **doc/coverage** - contains the code-coverage-report
* **vendor** - contains all the additional libraries that you imported
* **dist**  - contains the distribution-files of your project
* **tests** - containing your test-files

##Installation

Install it by creating a file called ```composer.json``` with the following
content:

```JSON
{
    "require-dev" : {
        "mdv/devpackages" : "dev-master"
    },
    "repositories": [{
        "type": "composer",
        "url": "http://packages.wdv.de/"
    }],
    "minimum-stability": "dev",
    "config" : {
        "bin-dir" : "bin"
    }
}
```

You can use the file ```example.composer.json``` as template.
