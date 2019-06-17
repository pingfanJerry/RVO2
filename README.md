# RVO2
Based On RVO2,more suitable for games

##Update
1. 添加碰撞处理,使得RVO2计算时,可以根据项目需要设置部分单位再避障时不考虑一些单位.    
2. 当工作线程为1时(默认为1),只使用主线程计算RVO结果,而不是从线程池里拿一个线程来运算.
3. 去掉因为完美对称性导致的单位死锁问题所增加的微调代码.(实际上没发现这问题.而且这里大量运用了浮点数和随机数,不太符合帧同步游戏需要,后面如果真遇到这问题了再修改为一个更合适的版本)
