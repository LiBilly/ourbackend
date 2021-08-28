# @Autowired @Resource @Inject

三者都是关于资源bean注入的注解

## @Autowired

Spring独有注解
默认按照类型ByType匹配，通过@Qualifier实现按照名称匹配
可以用于field，setter，constructor
Spring通过AutowiredAnnotationBeanPostProcessor实现的依赖注入

## @Resource

JSR250 javax.annotation, jdk9后需要加入依赖
默认按照名称匹配，其次按照类型
可以用于field，setter
Spring通过CommonAnnotationBeanPostProcessor实现的依赖注入

## @Inject

JSR330 Dependency Injection for Java，javax.inject, jdk9后需要加入依赖
可以用于field，setter，constructor
Spring通过AutowiredAnnotationBeanPostProcessor实现的依赖注入
除Spring,其他DI框架，比如Guice，也实现该注解