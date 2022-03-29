# cerberus-z80-forth
FORTH for the Z80 CPU of the Cerberus 208

This FORTH system is designed to run on the Z80 CPU of the Cerberus 2080
computer.

A useful introduction to FORTH can be found here. 
http://galileo.phys.virginia.edu/classes/551.jvn.fall01/primer.htm
The FORTH system does not have all features mentioned in that document, such
as local variables and floating point.

1.1 Package contents

The cerberus-z80-forth package  contains the following files.
- manual.txt (the user manual).
- forth80.bin (the FORTH binary to run on Cerberus-2080).
- COPYING (the GPLv3 license file).
- glossary.txt (a list of all words in FORTH with a short explanation).
- squares.4th (a short example program).
- primes.4th (a primes benchmark example).
- testcode.4th (example for code definitions).
- tester.4th and core.4th (a regression test suite). Note that this is
  by a different author and not covered by the GPLv3.
- glosgen.4th and doglos.4th  Tools used to generate the glossary.txt file.
  These cannot be run on Cerberus Z80 FORTH, but you can run them from gforth
  or any other ANSI standard FORTH with the FILE extension wordset.
- crossz80.4th Can be run from gforth to generate Cerberus Z80 FORTH from
  source.
- metaz80.4th. The metacompiler, used to generate Cerberus Z80 FORTH from
  source.
- asmz80.4th. Source of the FORTH assembler.
- asmtst80.4th assembler file containing all types of instructions. Can
    be cross assembled and then the output checked with a disassembler.
- editor.4th. Source of the FORTH editor.
- kernl80a.4th, kernl80b.4th, kernl80c.4th, and extend80.4th: sourcees of
  Cerberus Z80 FORTH.

1.2 Prerequisites

You need Dean Belfield's BIOS with additonal functions to load and save
files. If you run BBC Basic on the Z80, you will already have this.
https://github.com/breakintoprogram/cerberus-bbc-basic/tree/main/cat

You need to reprogram the CAT chip on your board with this version of BIOS
if you want to run Cerberus 2080 FORTH.
