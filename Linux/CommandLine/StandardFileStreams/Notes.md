# Types of filestreams
    1. standard input (stdin, Value:0, example: keyboard)
            general template willbe : do_something < input-file

    2. standard output(stdout, Value: 1, Eg: terminal)

            gen. template would be : do_something > input-file

                echo "Doing using terminal" > something.txt


    3. standard error(stderr, Value:2, eg: log file)
            do_something 2> error-file


    Special Thing:

        do_something > all-output-file 2>&1
        the above code will do Put BOTH successful output and errors into all-outfile.

        for eg 
        nodemon app.js > logs.txt 2>&1
        if nodemon app.js got error it will be printed in the log.txt(the mentioned one) file and if i runs it will shows the output too in that exact file 

# Finding File
    1. locate <zip> | grep <bin>