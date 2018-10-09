# C++11 Snippets

# Time since epoch (in ms)
```C++
auto start = std::chrono::system_clock::now();
std::time_t today_time = std::chrono::system_clock::to_time_t(start);
auto val = std::chrono::duration_cast<std::chrono::milliseconds>(start.time_since_epoch()).count();
```
