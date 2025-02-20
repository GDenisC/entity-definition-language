# Style of EDL

## 1. Tank Definition

```edl
tank MyTank { ... }
```

## 2. Gun Definition

```edl
gun MyGun { ... }
```

## 3. Gun Stats Definition

```edl
state MyGunStats {}
```

## 4. Types

### Number

It's just a number. Some examples: 1, 2, 3, 4, 5, -1, -2, -3, -4, -5, 0.1, 0.2, 0.25, 0.125, etc.

### String

String in EDL can be EndOfLine-terminated and default one.

```edl
"It's a normal string!"
It's a eol-terminated string!
```

### Expressions

You can use number expressions like this:

`1/2` = `0.5`
`1/3` = `0.33333333333...`
`1e10` = `10000000000`
`1e-10` = `0.0000000001`

### Constants

`pi` = `3.1415926535...`
`tau` = 2 * pi

### Functions

#### EDL build-in functions

`log(x: str): void` - logs the text in the console
`str(x: num): str`
`num(x: str): num`

#### Math functions

`sin(x: num): num`
`cos(x: num): num`
`tan(x: num): num`
`dist(x: num, y: num): num`
`pow(x: num, y: num): num`
`round(x: num): num`
`floor(x: num): num`
`ceil(x: num): num`
`abs(x: num): num`

## 5. Operators

### `+`

### `-`

### `*`

### `/`

### `%`

### `++`

### `--`

### `==`

### `!=`

### `>`

### `>=`

### `<`

### `<=`

### `&&`

### `||`

## 6. Loops

```edl
// Simple loop
loop (i = 0; i < 10; ++i) {
    print(i);
}

// Loop with step of 10
loop (i = 0; i < 100; i += 10) {
    print(i);
}

// Loop to calculate an angle for 16 guns
loop (a = 0; a < tau; a += tau / 16) {
    guns += MyGun : { angle = a }
}
```
