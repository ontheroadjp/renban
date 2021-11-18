# renban
This script is to rename files to sequential numbers in bulk



## Install

```bash
git clone https://github.com/ontheroadjp/renban.git
echo "PATH=path/to/clone/dir/renban:${PATH}"
```



## Usage

```bash
renban -e jpg
```

- At a minimum, specify the target file extension.
- Multiple file extensions can be set.



### Cold Run

You can check the execution result by giving the -cold-run option before actually renaming the file.

```bash
$ renban . -e jpg --cold-run
[renban] EXEC as COLD RUN >>>
[renban] ./Ep.CyL9gSs.jpg ===> ./000001.jpg
[renban] ./PjmnRkwEDa.jpg ===> ./000002.jpg
[renban] ./nqL3S\KZf+.jpg ===> ./000003.jpg
```



## Options

```bash
Options:
  -h, --help                     Show help
  -v, --version                  Show script version
  -e, --extension ARG            Specify the target file extension
  -r                             Subfolders will also be handled recursively.
      --cold-run                 Run as cold run. No actual file renaming
      --verbose                  Print various logging information
```

