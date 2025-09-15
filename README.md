## 0 - 1
Ler o arquivo readme na pasta home e salvar a senha ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If

## 1 - 2: Read a dashed `-` file
> This type of approach has a lot of misunderstanding because using - as an argument refers to STDIN/STDOUT i.e dev/stdin or dev/stdout .So if you want to open this type of file you have to specify the full location of the file such as ./- .For eg. , if you want to see what is in that file use cat ./-
263JGJPfgU6LtdEvgfWU1XP5yac29mFx

## 2 - 3: Spaces in filename
> Same logic from the previous, if you want to use special linux cli characters such as - or -- in a file name, just provide the full path to the file and also just scape spaces when present.
MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx

## 3 - 4: Hidden File
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ

## 4 - 5: Using command `file` to check readability of file
4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw

## 5 - 6: Using find with arguments
> The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

    human-readable
    1033 bytes in size
    not executable

### Solution:
```
find . -type f -size 1033c \! -executable -readable -exec file '{}' \; 
```
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
## 6 - 7: Using find with grep
> The password for the next level is stored somewhere on the server and has all of the following properties:

owned by user bandit7
owned by group bandit6
33 bytes in size

### Solution
```
find . -type f  -size 33c -readable -exec ls -l '{}' \; | grep "bandit7 bandit6"
```
### Password
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj

