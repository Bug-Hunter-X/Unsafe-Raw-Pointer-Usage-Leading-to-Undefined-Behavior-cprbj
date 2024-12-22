# Unsafe Raw Pointer Bug in Rust
This repository demonstrates a common error in Rust involving unsafe raw pointers and how to address it safely.

## Bug Description
The `bug.rs` file contains code that uses a raw pointer to modify a vector's elements. This approach is unsafe because it can lead to undefined behavior if the pointer is used after the vector's lifetime ends.  The code incorrectly modifies the memory even after the vector is out of scope.

## Solution
The `bugSolution.rs` file presents a safer alternative using references or borrowing to access and modify vector elements, ensuring memory safety without the risks associated with raw pointers.