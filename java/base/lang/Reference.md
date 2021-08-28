# Reference 引用

## Strong Reference 强引用
直接引用，最普通的引用方式  
**引用存在时，被强引用对象不能被垃圾回收**

```java
 Object obj = new Object();
```

## SoftReference 软引用
比强引用弱一级， 用来描述一些还有用，但非必需的对象  
**在系统将要发生内存溢出异常之前，将会把被软引用对象列进回收范围**

```java
 SoftReference<Object> s1 = new SoftReference<>(new Object());
```