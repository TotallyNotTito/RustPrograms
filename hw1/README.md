# HW1: Modulo Exponential

### Tito Reinhart

### Project Summary

This was a pretty fun, albeit slightly challenging project. I feel that it went ok and that the book was incredibly helpful in outlining the concepts necessary to figure out how to use Rust to calculate the result. One of the biggest challenges I faced, which I imagine is the point of this project (In rock climbing we call it the crux of a problem), was the error of overflowing the calculation of the answer. There is a RUST built-in, `.pow(u32)`, that will abstract the calculation of the exponent. However, given the project params, a u32 is not acceptable for this project. In calculating the result manually, I used a loop that would multiply the result by the base paramater N times. This however caused an error when running the standard tests provided. Even though passing the same args from the command line produced no error, running the tests caused the calculation to panic. After some Google-Fu, I foundan algorithm that uses a math hack to calculate the exponent faster. This change allowed for the tests to pass and as far as I've tested, a working program. Maybe there is an edge case I've missed, but I tried passing strings which give an error, and I have tried passing negatives, and also numbers larger than u64, which also triggers the assert! macros in the program. 

Looking forward to continuing my Rust journey!    
