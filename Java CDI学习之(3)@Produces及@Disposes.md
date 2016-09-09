## @Produces及@Disposes
  > 学习@Produces和@Disposes前先了解@PostConstruct和@PreDestroy,我们知道所有的jsf/jsp最终运行时，是直行背后的servlet.
  > Servlet构造函数调用后会自动执行带有@PostConstruct的方法，而Servlet卸载前自动执行带有@PreDestroy的方法.
  > Servlet加入了这两个注解后执行顺序为：服务器加载servlet-->servlet构造函数-->@PostConstruc方法（例如init）-->Service-->destroy-->@PreDe> stroy方法-->服务器卸载Servlet
