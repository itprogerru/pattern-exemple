#Одиночка (singleton)
Когда мы используем один экземляр объекта везде
```javascript 
class Singleton {
    static getInstannce() {
        if (!Singleton.instance) {
           Singleton.instance = new Singleton ();
        }
        return Singleton.instance;
     }
}     
```

```javascript 
class Singleton {
    static getInstannce() {
        if (!Singleton.instance) {
           Singleton.instance = new Singleton ();
        }
        return Singleton.instance;
     }
    constrructor() {
        if (!Singleton.instance) {
                Singleton.instance = new Singleton ();
        }
         return Singleton.instance;
    }
}     
```
###примущества

1. гарантирует наичие единственного экземпляра класа
2. глобальная точка доступа
3. реализует отлажаная инициализация объекта

*Сложно тестировать*

----

#Фабрика (factory)
