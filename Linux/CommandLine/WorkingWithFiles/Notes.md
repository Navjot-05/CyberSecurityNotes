# for Reading

    1. wc <filepathORName>  :   Shows the file datasize and details

        a. cat -n <filename/path> : Shows file content with mentioning number of lines
        b. to read data backwards down to upside use tac instead of cat


    2. less <filepathORName>:   Shows the files but one page at a time need to scroll using 'space' && use -N for making it mention no. of lines

# For Creating
    3. touch <filename> : to create an empty file for later purposes

    4.touch -t < Year2018Month04Day30TimeIn24hrsFormat10:15> : setting timestamp manually

# For Deleting/removing directory and files
    5. rmdir :to remove blank directory
        a.) rm -rf <DirName> : to delete directory with it's existing content (recursively) 


    6. rm   : to remove a file
        a.) rm -f <Filename>    (to remove forcefully)
        b.) rm -i <Filename>    (to remove interactively will need reassurance)

# For Renmae a file
    6. mv <OldFileName> <FileNameToBe>

    7. mv <OldDirectoryName> <DirectoryNameToBe>


# finding file using it's extension
    sudo find . -name "*.log"

    sudo find /usr -type f -name gcc
        in above -type f meant type of the one that we're finding is file
            d- directory
        and -name gcc meant it's name must be gcc
# to find and remove the file
    find -name "*.swp" -exec rm {} ';'

    To Find files based on the time
    find /{pathof the file} -ctime 3
    
    to find file based on the size of it
    find /{filePath} -size 0