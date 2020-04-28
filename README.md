# coverage-fixpaths

A small CLI tool that automatically fixes paths in Cobertura coverage reports.

## Usage

```
$ coverage-fixpaths --source /path/to/source/files coverage.xml
```

This tries to match the filenames in `coverage.xml` to the actual files in `/path/to/source/files`.
If they are all present on the file system, `coverage-fixpaths` replaces any common prefix in the coverage
report with  `/path/to/source/files` (or a subdirectory thereof, if needed).

The option `--source` defaults to `.` (i.e. the current working directory).


## Installation

```
pip install coverage-fixpaths
```
