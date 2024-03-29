# Media-Query-Mixin
My lovely media-query-mixin
* Use the variable as in many projects (small, medium, large)
* Futhermore each variable has two subdivisions, for higher detail (…_a, …_b)
* insert px accurate queries
* the mixin can also detect a touch device.

## How to use
Define your own divisions
* ```mq-a: 480px;``` (mq-a … mq-e) is a default var. So you can define your own division

The mixin "mq" has 5 options
1. choose a section like ```@include mq(medium)``` or ```@include mq(medium_b)```
2. choose a detailed section (with start and end) like ```@include mq(small_b,medium)```
3. choose a pixel-accurate implementation like ```@include mq(350px,805px)```
4. use in each option the key ```x``` for a open start or open end like ```@include mq(x,805px)``` or ```@include mq(medium_b,x)```
5. specify only ```touch``` and the styles applies only to mobile devices with touch function

## visual table
```
           a          b          c          d          e
|-----------------------------------------------------------------|
|0      479|480    767|768    949|950   1279|1280  1349|1350     ∞|
|----------|----------|----------|----------|----------|----------|
|        SMALL        |       MEDIUM        |        LARGE        |
|----------|----------|----------|----------|----------|----------|
| SMALL_A  | SMALL_B  | MEDIUM_A | MEDIUM_B | LARGE_A  | LARGE_B  |
|-----------------------------------------------------------------|
```

## License
Media-Query-Mixin is MIT licensed.
