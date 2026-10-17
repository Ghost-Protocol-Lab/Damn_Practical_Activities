# 61 — Build a Tiny Fuzzer and Point It at a CLI Tool You Own

## What to Do
Write a simple mutation-based fuzzer from scratch that generates malformed inputs and feeds them to a CLI tool, watching for crashes, hangs, or unexpected behavior. Use a tool you compiled yourself so you can also analyze any crashes with a debugger.

## Open Source Resources
- AFL++ (American Fuzzy Lop) — github.com/AFLplusplus/AFLplusplus
- libFuzzer (built into LLVM/clang)
- Boofuzz (Python network fuzzing framework) — github.com/jtpereyda/boofuzz
- Python's subprocess module (for rolling your own simple fuzzer)

## Tips
- Start by writing a 20-line Python fuzzer before touching AFL — building one from scratch teaches you what a fuzzer actually does.
- Compile your target with AddressSanitizer (`-fsanitize=address`) to catch memory errors that don't immediately crash the program.
- Seed your mutations from valid inputs — pure random inputs rarely reach interesting code paths.

## When It's Completed
Your fuzzer has run at least 10,000 iterations, you've found and can reproduce at least one crash or unexpected behavior, and you've identified the input that caused it.
