# Recursive Keyword Search Script

This script recursively searches for files with specified extensions and uses `grep` to print lines in those files that contain the specified keyword.

## Usage

```bash
./search_kw <grep_flags> ext_0 ext_1 ... keyword
```

For example, if you want to search the the keyword `mesh` in my header and source files, you will run:

```bash
./search_kw h cpp mesh
```
this will search (recursively) through all files ending with .h and .cpp and print out lines which contain the keyword `mesh`

You can specify any number of extensions. E.g., if you also want to search python files (.py)

```bash
./search_kw h cpp py mesh
```

If you want grep to ignore case—for example, to match both mesh and Mesh—you can pass the appropriate grep flag before specifying the extensions (in this case, -i).

```bash
./search_kw -i h cpp mesh
```


