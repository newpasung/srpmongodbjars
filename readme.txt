����srpmongodb.jar����Ҫ���룬������Ҫ���õİ�������ʱ��Ҫע�ⲻҪ���Ѵ��ڵİ��ظ���������������
�÷�����������

public static void main(String[] args) {
		// ����ΪxxxService��ʵ������Ϊ��Ӧ��xxxServiceImpl����
		UserService userService = new UserServiceImpl();
		// ���Դӿ���̨��������
		System.out.print(userService.register("accounta", "passworda"));
		// ������Ҫ��mongodb��ʱ���ͷŵ�mongodb��ע���ʼ�������ᱻ�Զ�ִ��
		MongoProxy.shutDown();
	}

