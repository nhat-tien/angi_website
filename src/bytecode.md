# Bytecode

## The format

## The opcode

- `LOAD_CONST  dr, const_offset`
- `NEW_OBJECT  dr`
- `SET_ATTR    dr, rKey, rValue`


```txt
port = 3030;
response.message = "Hello";

 1  2  3  4  5  6  7  8  9  10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32
|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|
|              |           |           |           |
     opcode       Des Reg         ...
```

## Section 

### In head
- Magic number(u32): 0x414E4749 = "ANGI"
- version(u16): 0x0001 = "0.0.1"
- const_offset(u32)
- const_size(u32)
- code_offset(u32)
- code_size(u32)


