2020.05.19

constructor
  1、不需要初始化state、绑定方法的时候不需要实现constructor方法;
  2、constructor在挂在前调用，如果是一个class 组件，应该在其他状态之前调用super(props),否则会是的this.props是undefined；
  3、constructor两个使用目的：初始化this.state, 给实例绑定方法；
  4、constructor中不能setState，如果需要使用state，直接给this.state赋值；
  5、constructor是可以直接定义state的唯一地方，在其他方法中可以使用setState方法来更新state；
  6、避免在constructor中引入副作用或者订阅，可以写在componentDidMount里面；


componentDidMount
  1、组件挂载完毕立即执行的方法、DOM节点的初始化在此处进行，也是获取后台返回数据的地方；
  2、

