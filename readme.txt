其中srpmongodb.jar是主要代码，其他需要引用的包，导入时需要注意不要与已存在的包重复，否则会引起错误。
用法简单例子如下

public static void main(String[] args) {
		// 声明为xxxService，实际类型为对应的xxxServiceImpl即可
		UserService userService = new UserServiceImpl();
		// 可以从控制台看见输入
		System.out.print(userService.register("accounta", "passworda"));
		// 当不需要用mongodb的时候释放掉mongodb，注意初始化工作会被自动执行
		MongoProxy.shutDown();
	}

