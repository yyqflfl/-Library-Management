#### 用vue做的一个简单的图书管理系统

![images](https://github.com/yyqflfl/Library-Management/blob/master/images/1.png)

用到的知识点:

​	// 过滤器:filter(格式化日期)

​    // 自定义指令:focus(表单自动获取焦点)

​    // 计算属性:computed(统计图书数量)

​    // 侦听器:watch(验证图书名是否存在)

​    // 生命周期:mounted(图书数据处理)

补充知识点:

1.变异方法(修改原有数据)

push()     pop()     shift()     unshift()     splice()     sort()     reverse()

2.替换数组(生成新的数组)

filter()     concat()     slice()

3.修改响应式数据

var vm = new Vue({

   el: '#app',

   data: {

​    list: ['apple', 'orange', 'banana'],

​    info: {

​     name: 'lisi',

​     age: 12

​    }

   },

  });

  // vm.list[1] = 'lemon';

  // Vue.set(vm.list, 2, 'lemon');

  vm.$set(vm.list, 1, 'lemon');



  // vm.info.gender = 'male';

  vm.$set(vm.info, 'gender', 'female');