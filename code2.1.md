# Data-Structure-Algorithm
# Code2.1

typedef int Rank; //定义秩
#define DEFAULT_CAPACITY 3 //设置初始容量为3

template <typename T> class Vector{ //定义一个向量的类模板
protected:
	Rank _size; int _capacity; T* elem; //规模、容量、数据区
	void copyForm ( T const* A, Rank lo, Rank hi ); //定义复制函数，复制数组区间为A[lo,hi)
	void expand; //定义扩容函数，空间不足时扩容
	void shrink; //定义压缩函数，装填因子过小时压缩
	bool bubble ( Rank lo, Rank hi); //定义扫描交换函数
	void bubbleSort ( Rank lo, Rank hi); //定义起泡排序算法的函数
	
	
    
