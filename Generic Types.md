## 泛型 `Generic Types`
1. 泛型是什么
> 泛型最精准的定义：参数化类型。具体点说就是处理的数据类型不是固定的，而是可以作为参数传入。定义泛型类、泛型接口、泛型方法，这样，同一套代码，可以用于多种数据类型。

2. 泛型类和泛型方法
   1. 泛型类和接口
   
      泛型类和接口类似，定义一个泛型类：
   ```$xslt
   public class Som<T> {
       private T value;
   
       public T getValue() {
           return value;
       }
   
       public void setValue(T value) {
           this.value = value;
       }
   }
   
   ```
    Som就是一个泛型类，value的类型是T，而T是参数化的。如果有多个类型参数，使用分号隔开,如<U,V>。
   
   使用泛型类：
	```$xslt
    Som<String> som = new Som<>();
    som.setValue("Hi");
    //som.setValue(123);编译不通过1
    String str = som.getValue();

类型安全：
类型不安全：
	1.泄露
		内存扫描
		内存泄漏
	2.调用时类型明确
泛型使用最多的是结合集合。HashMap一起使用