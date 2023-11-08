---
{"dg-publish":true,"permalink":"/main/blog-posts/2023-08-29-reversible-rust-reversible-computing-link-haven-t-read/","noteIcon":""}
---

#rust #reversible-computing #havent-read-yet #computer-science

[[2023-08-29\|2023-08-29]]

haven't read this yet, but it seems worth sharing.

https://blog.erk.dev/posts/rrust/

>  **Introduction**
> 
> **Reversible computing** is the idea that you can for a given function `f(x) := y` you can generate the inverse function that takes the output and generates the input `f^-1(y) := x`. This of course could be done by hand, but we want to make a machine, here donoted by I, that can make the transformation of the code. That is that `I(f) := f^-1`. To generalize this a bit we can look at `x` and `y` as states and `f` as a function that goes from state `x` to state `y`, this is how we will look at it in the following chapters since we are going to model our functions as mutations to variables. So we want to generate the inverse function `f^-1` that takes state y and mutates it to state x.

