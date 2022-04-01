Quick hack on the linux kernel [checkpatch.pl] to lint C files written
according to Drew Devault's [cstyle]

## Usage

```
./checkpatch.pl --no-tree --terse --file <file>
```

To batch-process, try something like:

```
find src/ -name "*.c" -type f -exec checkpatch.pl --terse --no-tree --file {} \;
```

```
for f in ./*.c
do
	checkpatch.pl --terse --no-tree --strict --file "${f}"
done
```


[checkpatch.pl]: https://github.com/torvalds/linux/blob/master/scripts/checkpatch.pl
[cstyle]: https://git.sr.ht/~sircmpwn/cstyle
