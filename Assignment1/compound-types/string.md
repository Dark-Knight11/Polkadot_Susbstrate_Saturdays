## Str and &str

1.
```rust
// Fix error without adding new line
fn main() {
    let s: &str = "hello, world";

    println!("Success!");
}
```

2.
```rust
// Fix the error with at least two solutions
fn main() {
    let s: Box<str> =  "hello, world".into();
    greetings(&s)
}

fn greetings(s: &str) {
    println!("{}",s)
}
```


## String
3.
```rust
// Fill the blank
fn main() {
    let mut s = String::new();
    s.push_str("hello, world");
    s.push('!');

    assert_eq!(s, "hello, world!");

    println!("Success!");
}
```

4.
```rust
// Fix all errors without adding newline
fn main() {
    let mut s =  String::from("hello");
    s.push(',');
    s.push_str(" world");
    s += &"!".to_string();

    println!("{}", s);
}
```

5.
```rust
// Fill the blank
fn main() {
    let s = String::from("I like dogs");
    // Allocate new memory and store the modified string there
    let s1 = s.replace("dogs", "cats");

    assert_eq!(s1, "I like cats");

    println!("Success!");
}
```
