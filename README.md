# MyCodingDiary
记录我的JAVA学习历程
### 2026.3.11 算法打卡：两数之和

今天成功解决了 LeetCode 第 1 题，并学会了如何精准控制 `break`。

#### 我的 Java 代码：
```java
//两数之和：
public class TwoSum {
    public static void main(String[] args) {
        //一个存储整数的nums数组
        int[] nums = new int[]{2, 7, 11, 15, 17, 18, 19, 3, 5};
        //设置目标值
        int target = 26;
        for (int i = 0; i < nums.length; i++) {
            for (int j = i + 1; j < nums.length; j++) {
                //如果这两个数的和为目标值，则输出这两个数的索引
                if (nums[i] + nums[j] == target) {
                    System.out.println(i + "," + j);
                    break;
                }
            }
        }
    }
}
