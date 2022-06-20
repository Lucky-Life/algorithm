class Solution {

  public int removeDuplicates(int[] nums) {

​    *//判断生成数组是否为空或长度为0*

​    *if*(nums == null || nums.length == 0){

​      *return* 0;

​    }*else*{

​      */\*创建节点：*

​        *back为起始点，front为目标节点*

​        *当front != back 时将值赋给back++后的 nums[back]*

​        *随后return数组元素个数*

​        **/*

​      int back = 0;

​      *for*(int front = 1;front < nums.length;front++){

​        *if*(nums[back] != nums[front]){

​          back++;

​          nums[back] = nums[front];

​        }

​      }

​      *return* back + 1;

​    }

  }

}