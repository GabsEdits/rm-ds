<div align="center">
  <h1>Remove DS_Store files</h1>
  <p>Remove all .DS_Store files from a directory</p>
</div>

## Installation

```bash
npm install -g rm-ds
```

## Usage

### Current directory

```bash
rm-ds
```

### Specific directory

```bash
rm-ds <directory>
```


Replace `<directory>` with the path to the directory you want to remove the `.DS_Store` files from.

## FAQ

### How did the project start?

I was tired of seeing `.DS_Store` files in my repositories, and running `find . -name '.DS_Store' -type f -delete` every time without getting an log of the files that were deleted. So, I created this project to solve that problem.

### Why is there an `rm-ds.sh` file and an `bin/rm-ds` file?

The `rm-ds.sh` file is just for me, so I can run the script without installing it globally. The `bin/rm-ds` file is the actual script that is installed globally. Both of them are the same, but the `rm-ds.sh` file is not installed globally.

### The name?

`rm-ds` stands for "remove .DS_Store". It's a simple name that describes what the project does.
