
https://leetcode-cn.com/problems/two-sum-ii-input-array-is-sorted/


```cpp

class Solution {
public:
    vector<int> twoSum(vector<int>& numbers, int target) {

        int i = 0, j = numbers.size() -1;
        while (i < j) {
            int cur = numbers[i] + numbers[j];
            if (cur == target)
                return { i + 1, j + 1};
            else if  (cur >  target) {
                j--;
            }
            else {i++;}
        }
        return {-1, -1};

    }
};
```

