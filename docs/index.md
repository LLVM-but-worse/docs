# Welcome to MapleIR
---

Maple-IR is an industrial IR-based static analysis framework for Java bytecode. Currently, it implements SSA-form based analysis as well as construction and destruction from bytecode to IR. The toolchain takes bytecode input, lifts it to SSA IR, transforms the IR, then recompiles back down to bytecode. This is done by symbolically executing each method while simulating the stack, similar to how Binary Ninja or IDA Pro's Hex-Rays operate. 


## Why use MapleIR over Soot?

MapleIR is designed to be a Java -> IR -> Java obfuscation resilient framework. This is pragmatically useful for individuals interested moreso in using IRs for the purpose of deobfuscation/obfuscation over analysis. Many features available in Soot/SootUp are not replicated and supported in MapleIR.

## Who uses MapleIR

- [Skidfuscator](https://github.com/skidfuscatordev/skidfuscator-java-obfuscator) (Java Obfuscator)
