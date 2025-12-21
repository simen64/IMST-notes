`sort` is a **text-processing command** that sorts **lines of text**.

It can sort numbers, words, or even the output from another command using the **pipe (`|`)** operator.

Think: _“Take whatever this command prints and line it up neatly in order.”_

When you use a **pipe (`|`)**, you’re telling the shell:

“Take the _output_ of the command on the left, and use it as the _input_ for the command on the right.”

| Flag   | Meaning                                          |
| ------ | ------------------------------------------------ |
| `-r`   | Reverse order                                    |
| `-n`   | Sort numerically                                 |
| `-h`   | Sort human-readable sizes (e.g. 1K, 1M)          |
| `-k N` | Sort by column N                                 |
| `-u`   | Unique lines only                                |
| `-t X` | Use `X` as column separator (e.g. `-t,` for CSV) |