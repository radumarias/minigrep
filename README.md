A very simple Rust sample binary app of a very simple grep-like util that uses the `regex` crate to match lines.\
First argument is the pattern to match, and the second is the filepath  to search in.\
By default it's case sensitive, but you can set the env var `IGNORE_CASE` (with any value) to make it case insensitive.\
It will print the lines that match the pattern.
\
\
It demonstrate usage of:
- command line arguments
- reading from files
- environment variables
- `eprintln!` macro for printing errors to `stderr`
- lifetime annotations
- `match` expression
- using iterators
- tests
- binary and library app structure

# Usage
```
minigrep test file.txt
```
case insensitive
```
IGNORE_CASE=1 minigrep test file.txt

```