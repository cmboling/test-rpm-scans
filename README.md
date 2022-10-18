# test-rpm-scans
Testing out RPM scanning

`fossa-deps-conversion.py` will convert `artifacts.json` into referenced dependencies and it will also convert all .rpm and .tar files in the current directory.
After that is complete, the FOSSA CLI will recognize that a `fossa-deps.json` was created and will consider it a target for analysis.

This is useful for those that don't want to include the  `fossa-deps.yml|json` in the repo; rather this method will dynamically create the `fossa-deps.yml|json` in the pipeline.
