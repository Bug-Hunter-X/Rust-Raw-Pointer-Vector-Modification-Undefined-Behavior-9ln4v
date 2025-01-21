# Rust Raw Pointer Vector Modification Undefined Behavior

This repository demonstrates a common error in Rust involving the unsafe use of raw pointers with vectors. Modifying a vector's contents via a raw pointer after operations that might reallocate the vector's underlying memory leads to undefined behavior, potentially causing crashes or subtle data corruption.

The `bug.rs` file contains the problematic code. The `bugSolution.rs` file provides a safe alternative using vector indexing or iterators.