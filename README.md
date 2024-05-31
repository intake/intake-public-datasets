# public-datasets

Intake catalogs pointing to freely available data


### To access public data

You will need Intake installed. Additionally, most catalogs will require other
packages to run, and these should be listed in either a catalog-wide, or
per-reader metadata field called "environment".

To load the root catalog:

```python
import intake
cat = intake.readers.PublicCatalogReader().read()
```

This reference to public data could also be embedded into other catalogs. 

### To add new catalogs

Note that neither Intake nor this host the data, any users will always fetch it
from the original location. If this requires some sign-up or credentials, this
should be indicated in the catalog description.

Create catalogs using Intake, and save them to YAML files. If you don't know how
to do this, please see the Intake tutorials and documentation. Please edit the
metadata to be as comprehensive as possible, and include license and attribution
information.

Clone and fork this repo, and make a PR adding the file to the catalog_files
directory, and the name of the file to the manifest.text file on a line
by itself.
