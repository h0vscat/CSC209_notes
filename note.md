# CSC209

## Week 1 _Shell and File Systems_

### __Unix manual__

    head, tail, cd, mkdir, ls, cp, mv, rm, diff, comm, cut, cat, wc, grep, who

### __Shells__

    $ gcc
    $ screen (?)

* $ is a shell prompt
* Shells
  * accept commands (programs) as input
  * finds the executable
  * interprets the arguments
  * starts executing the command

> environmental variable?

To run some program directily?

    $ export (?)
    $ echo (?)

### __File and Directories__

directories is not regular file
executable file

### __Directories and links__

### __Permissions__

-rwx (user) r-x (group) r-x (other)

### __chmod__

    chmod 755 <filename>

* 3 numbers between 0 and 7, the octal value of that category of user
* Another approach

```
chmod u+rwx
chmod go-x
```

### __Globbing__

* like regular expressions but different synatax
* \* matchs any number of any character
* ? matches any one character
* [list of characters]
* [1-5] or [a-z] or [a-xz]

> pointer types regular files??

---

## Week 2 _Arrays and Pointers_

```c    
int main() {
    int num = 40;
    int *pt;

    pt = &num;
    int *anotherpt = &num;

    *pt = 30;
    printf("%d\n", *anotherpt);

    return 0;
}
```

