# ES6 spread operator
总结ES6的扩展运算符

### 函数调用中使用扩展运算符
将一个数组展开成多个参数
  
      function test(){}
      let a = [1,2,3];
      test(...a) // 相当于 test（1,2,3）
      
### 数组字面量中使用扩展运算符
1.在ES6 的世界中，我们可以直接将一个数组合并到另一个数组中

      let arr1 = [1,2,3,4];
      let arr2 = [6,...arr1,8];//[6,1,2,3,4,8];
      
2.将两个数组合并成一个

      let arr1 = [1,2];
      let arr2 = [3,4];
      let arr3 = [...arr1,...arr2]; // [1,2,3,4]

3.展开运算符也可以用在push函数中，可以不用再用apply()函数来合并两个数组

      let arr1 = [1,2];
      let arr2 = [3,4];
      arr1.push(...arr2); //[1,2,3,4]
      
### 用于结构赋值
 
      let [arg1,arg2,...arg3] = [1, 2, 3, 4];
      arg1 //1
      arg2 //2
      arg3 //['3','4']
     
     
### ES7 草案中关于扩展运算符
  
  1.合并对象
