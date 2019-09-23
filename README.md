# php-path-testdome

**BEST ANSWER EVER** - Write a function that provides change directory (cd) function for an abstract file system

- The question is originated from [PHP TESTDOME](https://www.testdome.com/questions/php/path/7265?testId=30&testDifficulty=Hard)
- The general solution is accepted as this [Github Gist](https://gist.github.com/TheRealJAG/0acc8b81be8012f14a6b58808a0de26d), but it's not a completion yet.
- `¯\_(ツ)_/¯`
- This would be my best solution for the question ever.

## Description:
```
Root path is '/'.
Path separator is '/'.
Parent directory is addressable as '..'.
Directory names consist only of English alphabet letters (A-Z and a-z).
The function will not be passed any invalid paths.
Do not use built-in path-related functions.
```

## Expectation:
```php
$path = new Path('/a/b/c/d');

$path->cd('../x');
echo $path->currentPath;
# should display '/a/b/c/x'.

$path->cd('./x');
# should display '/a/b/c/d/x'.

$path->cd('x');
# should display '/a/b/c/d/x'.

$path->cd('/a');
# should display '/a'.

$path->cd('../../e/../f');
# should display '/a/b/f'.

$path->cd('/d/e/../a');
# should display '/d/a'.
```
