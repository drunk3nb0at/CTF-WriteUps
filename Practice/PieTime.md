* Not original, solution is fully referred from [PIE TIME — picoCTF 2025 by Jin from Medium](https://systemweakness.com/pie-time-picoctf-2025-dbec42ba0857)

```shell
wget https://challenge-files.picoctf.net/c_rescued_float/{instance}/vuln.c # or just download lol

wget https://challenge-files.picoctf.net/c_rescued_float/{instance}/vuln

chmod +x vuln # remember to change mode to execute

./vuln

nano vuln.c

gcc vuln.c -o vuln1 # compile to executable

./vuln1

gdb ./vuln # start gnu debugger

(gdb) run 

(gdb) disas main # disassem [addr] display main memory as machine instructions

(gdb) disas win

```

```python
# 150 address offset
main = input("Enter hex: ")
main = int(main, 16) - 150
main = hex(main)
print(main)
```
