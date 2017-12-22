# Singleton
a singleton script for Unity

Create your class 
```c#
public class MyClass : Singleton<MyClass>
```

and create the static instance
```c#
public static MyClass instance { get{ return ( (MyClass) base.instance); } }
```
