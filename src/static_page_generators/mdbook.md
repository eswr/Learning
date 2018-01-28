# mdbook

## Commands

An nginx server for SSL termination which has a public address of 192.168.1.100 on port 80 and proxied that to 127.0.0.1 on port 8000, should run:

```bash
mdbook serve path/to/book -p 8000 -i 127.0.0.1 -a 192.168.1.100 -w 3000
```

**-o --open** : mdbook will open the book in your your default web browser after starting the server

**-w** : 192.168.1.100:<WS_PORT> will be proxied for live reload

#### Handy commands

```bash
mdbook test
mdbook serve
```

## Features

- syntax highlighting
- annotated `rust` code
```rust
# fn main() {
    let x = 5;
    let y = 6;

    println!("{}", x + y);
# }
```
- editable
```rust,editable
fn main() {
    let number = 5;
    print!("{}", number);
}
```
- can use runnable rust file via playpen
