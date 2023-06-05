[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/alploskov/rubik/blob/master/LICENSE.txt)

**rubik** is just for fun project for write C/C++ programs in ruby-like language


Quick start
-----------

Copy `rubik.h` to your project.


```ruby
// main.crb
#include <stdio.h>
#include "rubik.h"

main
    i32 i = 0;
    for i in range(10) do
        if i % 2 == 0 then
	    continue
	elsif i % 9 == 0 then
	    break
	end
        printf("%d\n", i);
    end
    return 0;
end
```


```
$ gcc -xc main.crb -o main
$ ./main
1
3
5
7
```
