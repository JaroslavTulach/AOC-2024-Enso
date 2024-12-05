# Enso Advent of Code 2024

[![CI](https://github.com/JaroslavTulach/AOC-2024-Enso/actions/workflows/enso.yml/badge.svg)](https://github.com/JaroslavTulach/AOC-2024-Enso/actions/workflows/enso.yml)

Solving tasks for [AoC 2024](https://adventofcode.com/2024) in [Enso](http://enso.org).

## Setup & Execution

First of all get this repository to your local computer. Use `git` to clone it:
```bash
$ git checkout https://github.com/JaroslavTulach/AOC-2024-Enso.git
$ cd AOC-2024-Enso
$ ls -1
Dec01
Dec02
Dec03
Dec04
Dec05
README.md
```
Let's download [Enso](http://enso.org) now. 
Enso can run on Linux, Windows, MacOSX. Download correct `enso-launcher` package
for your operating system. Use version [2024.4.2](https://github.com/enso-org/enso/releases/tag/2024.4.2).
The following steps are tested on Linux, but shall work on Mac too. They may need some modification on Windows:
```bash
$ wget https://github.com/enso-org/enso/releases/download/2024.4.2/enso-launcher-2024.4.2-linux-amd64.tar.gz
$ tar fxvz enso-launcher-2024.4.2-linux-amd64.tar.gz
$ ./enso/bin/ensoup install engine 2024.4.2
$ ./enso/bin/ensoup list
Enso 2024.4.2 -> GraalVM 24.0.0-java21.0.2
```
Now you can select an existing project and execute it. To execute for example `Dec03` invoke:
```bash
$ ./enso/bin/ensoup run Dec03
[INFO] [2024-12-05T16:05:26.396] [org.enso.interpreter.runtime.DefaultPackageRepository] Found library Standard.Base @ 2024.4.2 at [***/2024.4.2].
[INFO] [2024-12-05T16:05:26.462] [org.enso.interpreter.runtime.DefaultPackageRepository] Found library Standard.Table @ 2024.4.2 at [***/2024.4.2].
[INFO] [2024-12-05T16:05:26.481] [org.enso.interpreter.runtime.DefaultPackageRepository] Found library Standard.Database @ 2024.4.2 at [***/2024.4.2].
[INFO] [2024-12-05T16:05:26.498] [org.enso.interpreter.runtime.DefaultPackageRepository] Found library Standard.AWS @ 2024.4.2 at [***/2024.4.2].
[INFO] [2024-12-05T16:05:26.508] [org.enso.interpreter.runtime.DefaultPackageRepository] Found library Standard.Google_Api @ 2024.4.2 at [***/2024.4.2].
[INFO] [2024-12-05T16:05:26.517] [org.enso.interpreter.runtime.DefaultPackageRepository] Found library Standard.Snowflake @ 2024.4.2 at [***/2024.4.2].
[INFO] [2024-12-05T16:05:26.522] [org.enso.interpreter.runtime.DefaultPackageRepository] Found library Standard.Examples @ 2024.4.2 at [***/2024.4.2].
[INFO] [2024-12-05T16:05:26.527] [org.enso.interpreter.runtime.DefaultPackageRepository] Found library Standard.Visualization @ 2024.4.2 at [***/2024.4.2].
[INFO] [2024-12-05T16:05:26.806] [org.enso.interpreter.runtime.DefaultPackageRepository] Found library Standard.Image @ 2024.4.2 at [***/2024.4.2].
/home/devel/enso-projects/AoC2024/Dec03/src/Main.enso:29:5: warning: Unused variable integer1.
   29 |     integer1 = any3.length
      |     ^~~~~~~~
/home/devel/enso-projects/AoC2024/Dec03/src/Main.enso:42:5: warning: Unused variable prod1.
   42 |     prod1 = Main.evaluate any4
      |     ^~~~~
/home/devel/enso-projects/AoC2024/Dec03/src/Main.enso:43:5: warning: Unused variable any5.
   43 |     any5 = node1.compute ..Sum
      |     ^~~~
2
```
Enjoy!
