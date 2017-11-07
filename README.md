# Media-Query-Mixin
My lovely media-query-mixin
* Use the variable as in many projects (small, medium, large)
  Futhermore each variable has two subdivisions, for higher detail (…_a, …_b)
## How to use
The mixin "mq" has 4 options
1. choose a section like "@include mq(medium)" or "@include mq(medium_b)"
2. choose a detailed section (with start and end) like "@include mq(small_b,medium)"
3. choose a pixel-accurate implementation like "@include mq(350px,805px)"
4. use in each option the key "x" for a open start or open end like "@include mq(x,805px)" or "@include mq(medium_b,x)"
## visual table
```
|-----------------------------------------------------------------|
|0      479|480    767|768    949|950   1279|1280  1349|1350     ∞|
|----------|----------|----------|----------|----------|----------|
|        SMALL        |       MEDIUM        |        LARGE        |
|----------|----------|----------|----------|----------|----------|
| SMALL_A  | SMALL_B  | MEDIUM_A | MEDIUM_B | LARGE_A  | LARGE_B  |
|-----------------------------------------------------------------|
```
## Notice
Make sure you have an em calculator. Of course, you can use this awesome feature with "px" (you have to rewrite the mixin), but i've read a [revealing article](https://zellwk.com/blog/media-query-units/) by [zellwk](https://github.com/zellwk).
------------------
Made with ♥ by [chrstn-hsbrg](https://github.com/chrstn-hsbrg)
