# [RSA Factoring Challenge](https://github.com/leulyk/RSA-Factoring-Challenge)

<p float="left">
<img src="https://lh3.googleusercontent.com/oVJxT1yn7vwaEM8t9A5MGL6emG0j-_uqHa5H8ikWLvl6Ka-nVmUJZblqWDqPiY-S6itPLnZNgcc8rviK8AVT65l_a3zHiyctwy8=s0" width="245" height="150"/>
<img src="https://blog.holbertonschool.com/wp-content/uploads/2019/04/instagram_feed180.jpg" width = "150" height="150"/>
</p>


## Tasks

### 0. [Factorize all the things!]()

Factorize as many numbers as possible into a product of two smaller numbers.

    Usage: factors <file>
        where <file> is a file containing natural numbers to factor.
        One number per line
        You can assume that all lines will be valid natural numbers greater than 1
        You can assume that there will be no empy line, and no space before and after the valid number
        The file will always end with a new line
    Output format: n=p*q
        one factorization per line
        p and q don’t have to be prime numbers
        See example
    You can work on the numbers of the file in the order of your choice
    Your program should run without any dependency: You will not be able to install anything on the machine we will run your program on
    Time limit: Your program will be killed after 5 seconds if it hasn’t finish
    Push all your scripts, source code, etc… to your repository
        we will only run your executable factors

**Example:**

        julien@ubuntu:~/factors$ cat tests/test00 
        4
        12
        34
        128
        1024
        4958
        1718944270642558716715
        9
        99
        999
        9999
        9797973
        49
        239809320265259
        julien@ubuntu:~/factors$ time ./factors tests/test00
        4=2*2
        12=6*2
        34=17*2
        128=64*2
        1024=512*2
        4958=2479*2
        1718944270642558716715=343788854128511743343*5
        9=3*3
        99=33*3
        999=333*3
        9999=3333*3
        9797973=3265991*3
        49=7*7
        239809320265259=15485783*15485773

        real    0m0.009s
        user    0m0.008s
        sys 0m0.001s

### 1. [RSA factoring challenge]()

RSA Laboratories states that: for each RSA number n, there exist prime numbers p and q such that

n = p × q. The problem is to find these two primes, given only n.

This task is the same as task 0, except:

    p and q are always prime numbers
    There is only one number in the files

How far can you go in less than 5 seconds?
