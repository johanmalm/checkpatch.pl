This projects has migrated to the `scripts` folder of https://github.com/labwc/labwc


Quick hack on the linux kernel [checkpatch.pl] to lint C files written
according to Drew Devault's [cstyle]

## Usage

```
./checkpatch.pl --no-tree --terse --strict --file <file>
```

To batch-process, try something like:

```
find src/ -name "*.c" -type f -exec checkpatch.pl --no-tree --terse --strict --file {} \;
```

```
for f in ./*.c
do
	checkpatch.pl --no-tree --terse --stric --file "${f}"
done
```


[checkpatch.pl]: https://github.com/torvalds/linux/blob/master/scripts/checkpatch.pl
[cstyle]: https://git.sr.ht/~sircmpwn/cstyle
