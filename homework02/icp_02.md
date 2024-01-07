# 第二讲 作业2
## 实现公共接口 `public func qsort(arr: [Int]): async [Int]` （3 分）

### 代码
`main.mo`
```Motoko
    public func qsort(arr: [Int]) : async [Int] {
        var newArr:[var Int] = Array.thaw(arr);
        quicksort(newArr, 0, newArr.size()-1);
        Array.freeze(newArr)
    };
```
