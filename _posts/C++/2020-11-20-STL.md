## STL
### inserter

###  X适配器
1. ostream_iterator
    1. 重载了 =；++操作符；
    2. 修饰了 basic_ostream
2. istream_iterator
    1. 修饰 basic_istream
将具有重复行为的对象进行封装，以迭代的形式表现出来；


### hash Function
1. 基于各种类型的hash仿函；构造特定类型的仿函；
2. 通过"..." 传递不定量参数，实现参数拆解递归；
    void hash_val(size_t& seed, T val, T... args) {
    hash_combine(seed, val)
    hash_val(seed, args); //拆解参数递归；
    }
   
 ### Tuple
 1. 内部结构是层层继承；


### type traits



### movable
对vector而言：move construct 比 copy construct快（实际差距取决于内存破损程度）
list、deque、set：两者差距不大；
M c11(c1);
M c12(std::move(c1)); 浅拷贝；
1. move之后，不要再使用；


