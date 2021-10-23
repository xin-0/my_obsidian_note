---

---
# Multithread
reference: https://mp.weixin.qq.com/s/AP1AkvxcGG5DQ8557CvQ-Q
## Pthread
```cpp
class helloFromObject{
public:
	void operator()() const{
		std::cout << "Hello, My Second thread!" << std::endl;
	}
};

int main() {
	std::cout << "Hello, Coconut Cat!" << std::endl;
	std::thread bthread((helloFromObject()));
	bthread.join();
	return 0;
}
```


## OpenMP
