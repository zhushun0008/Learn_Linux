### Shell

1. test
use ***test*** to determine whether a directory or files, return ***0*** for success otherwise for failure
2. da
3. dsd
4. dad
5. dss
6. 

#### Problem Solved
1. 脚本传参遇到空格，会被截取
  * reference
    * [Shell脚本传递带有空格的参数](Shell脚本传递带有空格的参数)
    * [ shell参数传递 含有空格的问题 二楼回复](http://bbs.chinaunix.net/thread-4094745-1-1.html)
  * 可以使用 ***双引号或者${@:3}***
  * e.g.
  ```
    id2=1525
    id3=7057
    train_month_duration_for_user_buying="2016-03 2016-04 2016-05"
    
    # sh gen_train_user_pin.sh ${id2} ${id3} "$train_month_duration_for_user_buying" 
    # sh gen_train_user_pin.sh ${id2} ${id3} "${@:3}" 
  ```
