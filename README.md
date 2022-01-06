
![N|Solid](https://techrocks.ru/wp-content/uploads/2020/08/solid.png)
##### SOLID — это аббревиатура пяти основных принципов проектирования в объектно-ориентированном программировании.

Аббревиатура SOLID была предложена Робертом Мартином, автором нескольких книг, широко известных в сообществе разработчиков. 
## Для чего нужны Solid принципы: 
- Программу легко дополнять;
- Программу легко расширять;
- Программу легко поддерживать;
- Код будет легко читать;
- В коде будет легко находить ошибки;
#
#
![N|Solid](https://user-images.githubusercontent.com/45273279/140934003-5d14f08e-944f-400d-9dd5-511377b08368.png)
 > Принцип единой ответственности. Класс должен заниматься чем-то одним. Должна быть одна ось изменений. Если мы что-то меняем в классе и приходиться переписывать логику, то это нарушение прицепа единой ответственности.
#
#
![N|Solid](https://user-images.githubusercontent.com/45273279/140938622-a5610ba8-93ee-4d65-9d52-37bb8cb3d923.png)
>Принцип закрытости и открытости. Открыт для расширений, закрыт для изменений. Расширение происходит через наследование. 
#
#
![N|Solid](https://user-images.githubusercontent.com/45273279/140944144-2b1e3038-85b6-404a-842f-7cb798ea3fc2.png)
>Подклас не должен требовать от вызываемого кода больше чем базовый класс и не должен предоставлять вызывающему коду меньше чем базовый класс. Не ломать логику родительского класса.
#
#
![N|Solid](https://user-images.githubusercontent.com/45273279/140951313-d8bfec25-3da1-4e0d-8929-8952b45d5352.png)
> Клиент не должен зависеть от методов, которые они не используют. Протоколы не должны состоять из 100500 методов, потому что где-то они будут не использоваться.
#
#
![N|Solid](https://user-images.githubusercontent.com/45273279/140958814-cf7b5546-5c94-42bb-a9b4-d6a2f2f0e569.png)
>Принцип инверсии зависимостей. Модули верхних уровней не должны зависеть от модулей нижних уровней.
```swift
protocol Repo{
    func get()
    func del()
}
class NoteRepo: Repo{
    func get() {}
    func del() {}
}
class MyClass{
    var repo: Repo = NoteRepo()
}
```


**BB!**


