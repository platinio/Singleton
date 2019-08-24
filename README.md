Quickstart
==============
Just download and import [this](https://github.com/platinio/Singleton/releases/download/1.0.1/singleton.unitypackage) 

And don't forget to use the namespace

```c#
using Platinio;
```

Creating My Singleton
==============
Creating a singleton now is very easy, just create your class and extend from Singleton.

```c#
using UnityEngine;
using Platinio;

public class MyAwesomeSingleton : Singleton<MyAwesomeSingleton>
{    
}
```

And dont forget to override the Awake and OnApplicationQuit methods, if you need them, so everything can works as expected.

```c#
using UnityEngine;
using Platinio;

public class MyAwesomeSingleton : Singleton<MyAwesomeSingleton>
{
    protected override void Awake()
    {
        base.Awake();
        //do something
    }

    protected override void OnApplicationQuit()
    {
        base.OnApplicationQuit();
        //do something
    }
}

```
