## Dart 

- 级联 [操作符..]

链式调用的一种语法糖，例如：

```Dart
class A{
    String value1;
    String value2;
}

main() {
    A()
    ..value1 = "111"
    ..value2 = "222"
}
```

相对应java如下：
```java
class A{
    private String value1;
    private String value2;

    public A setValue1(String value1) {
        this.value1 = value1;
        return this;
    }

    public A setValue2(String value2) {
        this.value2 = value2;
        return this;
    }

    public static int main() {
        A a = new A();
        a.setValue1("111")
         .setValue2("222");
    }
}
```
