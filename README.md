2020.05.19

constructor
  1、不需要初始化state、绑定方法的时候不需要实现constructor方法;
  2、constructor在挂在前调用，如果是一个class 组件，应该在其他状态之前调用super(props),否则会是的this.props是undefined；
  3、constructor两个使用目的：初始化this.state, 给实例绑定方法；
  4、constructor中不能setState;
  5、
