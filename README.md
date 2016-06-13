# sphinx-doc

Docker image for building documentation via [Sphinx](http://www.sphinx-doc.org/).

This image has been primarily created for generating PDF documentation
via LaTeX, but may support other builders as well.

If you have a need to use it with a builder that is currently not supported
by this Docker image feel free to open a PR that adds the necessary packages.


## Usage

```bash
docker run -v <docs-directory>:/docs benjixx/sphinx-doc make <sphinx-make-target>
```


## Examples

Create HTML documentation:

```bash
docker run -v path/to/your/sphinx/docs:/docs benjixx/sphinx-doc make html
```

Create PDF documentation with the help of LaTeX:

```bash
docker run -v path/to/your/sphinx/docs:/docs benjixx/sphinx-doc make latexpdf
```
