# Search_kw
This code print recursively search for files with specified extension and use grep to print out lines in text files that contain the specified keyword.

To run, do:
    ```
    ./search_kw <grep flags> ext_0 ext_1 ... keyword
    ```

E.g. if I want to search the the keyword `mesh` in my header and source files, I will run:
    ```
    ./search_kw h cpp mesh
    ```
this will search (recursively) through all files ending with .h and .cpp and print out lines which contain the keyword `mesh`

I can specify any number of extensions. E.g., if I also want to search python files (.py)
    ```
    ./search_kw h cpp py mesh
    ```

If I want the case to ignore case, e.g., checking for both `mesh` and `Mesh` then I can pass the appopriate grep flag before specifying the extension (`-i` in this case)
    ```
    ./search_kw -i h cpp mesh
    ```


