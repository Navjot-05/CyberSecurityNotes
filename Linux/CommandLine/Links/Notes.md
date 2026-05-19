# Hardlinks 
    1. SYNTAX to create hard link is   ln file1.exe file2.exe

    2. Syntax to list the inode number (reltn with both the files) 

    3. think of the pointer used in the Memory that you've learnt at BCA

    4. it's basically the two file that points to the same data 

    5. you first create data in that file 
        a. echo "This is for creating an example" > original.txt


        Now we'll link the original.txt file with another one
        b. ln original.txt hardlink.txt

# Hardlink properties
    even if we remove any one file it will still points to the data via another filename
    if we change one file the another file will also gets changed

# Difference between hardlinks and symlinks(softLinks) is in the DiffHard_symlinks.png file 


# SoftLink (symlinks)
    1. Syntax :
                <!-- Note: file that is going to be used as softlink must be created before use -->
        ls file1 file3
    2. Syntax for inode no. checking
        ls -li file1 file3
    ~ PROPERTIES:
        a. it doesnot gets changed on changing it's other file that has the same content written in both
        b. crossplatform : ✅
        c. these links can point to the files even you are running any other platform 

    