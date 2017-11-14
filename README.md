# UsefulHelpFiles

to have ask cmake create Makefile with debug features.

```
mkdir Debug
cd Debug
cmake -DCMAKE_BUILD_TYPE=Debug ..
make
```
```
 sudo apt-get install openssl
```
https://www.howtogeek.com/278152/how-to-update-the-windows-bash-shell/

Code debugging.

http://www.cplusplus.com/forum/articles/28767/

multi thread debugging.
http://www.drdobbs.com/cpp/multithreaded-debugging-techniques/199200938

Debugging Strategies, Tips, and Gotchas

https://www.cprogramming.com/debugging/debugging_strategy.html


https://accu.org/index.php/journals/423

https://stackoverflow.com/questions/1325853/what-are-your-favorite-debugging-techniques-in-c

Path planning related:
https://www.researchgate.net/publication/267596342_Path_Planning_for_Collision_Avoidance_Maneuver
https://www.hindawi.com/journals/jr/2016/9329131/
https://robotics.stackexchange.com/questions/8555/which-trajectory-planning-algorithm-for-minimizing-jerk


Hex to string conversion in C#

string s = String.Concat(buffer.Select(b => b.ToString("X2")));

Moving standar variance
http://jonisalonen.com/2014/efficient-and-accurate-rolling-sta
ndard-deviation/


```Python
class RollingStatistic(object):

    def __init__(self, window_size, average, variance):
        self.N = window_size
        self.average = average
        self.variance = variance
        self.stddev = sqrt(variance)

    def update(new, old):
        oldavg = self.average
        newavg = oldavg + (new - old)/self.N
        self.average = newavg
        self.variance += (new-old)*(new-newavg+old-oldavg)/(self.N-1)
        self.stddev = sqrt(variance)

```
