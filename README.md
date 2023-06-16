# anticheat.c ⚡
Lightweight performant anti-cheat written in C.

File verification tool which performs over 62% faster than standard file verification protocol.

# Benchmarks

Standard File DFS and Hash time Benchmark (non-threaded-impl branch):

![image](https://github.com/PoromKamal/anticheat.c/assets/62628923/05a8e79b-e232-48bd-9e5a-04638691832d)


anticheat.c threaded DFS and Hash time benchmark:

![image](https://github.com/PoromKamal/anticheat.c/assets/62628923/9b0e464d-7c94-4906-b8e0-b9d7d6c3ee60)


Summary:

62+% increase in performance for large file systems

# Usage
1. To generate expected hashes (first time setup)
```
anticheat-dev <game_directory> -g
```

Remember to drag in verification.txt file (generated by the tool) into your game directory,
and ship with the verification.txt file

2. To verify files
```
anticheat-dev <game_directory> -v
```
Will exit with code:

0 - Verification Success

3 - Unsuccessful (Tampered files)

# Build instructions
In project root run:
```
make
```
To build the tool.

# Running Benchmarks
To run timing benchmarks (For Multithreaded version only):
(Run command first time only, requires around 100mb of space)
```
./timeBenchmark -setup
```
(Simply generates the expected hashes, performance wasn't considered at this step, so no multithreading)
```
./timeBenchmark -g
```
(Now can time the verification step, which is threaded)

```
./timeBenchmark -v
```
# Look at this Nehal guy 💀

![image](https://github.com/PoromKamal/anticheat.c/assets/62628923/90d31fe8-df13-48a8-ada7-fc6240060856)

Bro is in my backpack 😭

<sub><sup>jk proud of you lil bro <3 </sup></sub>
