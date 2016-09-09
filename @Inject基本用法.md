## @Inject基本用法
  - Filed Dependency injection
    public class SomeBean{
    
      @Inject
      private SomeService someService;
      
      ...
    }
  - Constructor Dependency injection
    public class SomeBean{
      
      private final Service service;
      
      @Inject
      public SomeBean(Service service){
        this.service = service;
      }
      
      ...
    }
  - Initializer methods Dependency injection
    public class SomeBean{
      
      private Service service;
      
      @Inject
      public void setService(Service service){
        this.service = service;
      }
      
      ...
    }
