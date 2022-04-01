Quick hack on the linux kernel [checkpatch.pl] to lint C files written
according to Drew Devault's [cstyle]

Run with

```
./checkpatch.pl --no-tree --terse --file <file>
```

[checkpatch.pl]: https://github.com/torvalds/linux/blob/master/scripts/checkpatch.pl
[cstyle]: https://git.sr.ht/~sircmpwn/cstyle
