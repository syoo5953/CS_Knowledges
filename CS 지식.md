## 클래스 VS 구조체

In Java, a class is a blueprint for creating objects, while a struct is a value type that can contain a group of fields. In general, classes are used to represent more complex entities that have both data and behavior, while structs are used to represent simple data structures that only contain data.
Here are some key differences between classes and structs in Java:

- Classes are reference types, while structs are value types. This means that when you pass an object of a class to a method, you are passing a reference to the object, while when you pass a struct to a method, you are creating a copy of the struct and passing it to the method.
- Classes can have constructors, destructors, and other methods, while structs cannot.
- Classes can be inherited from other classes, while structs cannot be inherited.
- Structs are typically used to represent simple data structures, such as a point in 2D space or a customer record, while classes are used to represent more complex entities that have both data and behavior.
- Overall, the choice between using a class or a struct in Java will depend on the specific requirements of your application and the nature of the data you need to represent.

### 값 타입

변수를 할당하면 스택 영역에 값이 저장된다.
변수를 복사한 후 복사본을 변경하더라도 원본에 영향을 주지 않는다.
힙 영역을 사용하지 않고 레퍼런스 카운팅이 필요하지 않다.

 
### 참조 타입

스택 영역에는 포인터(레퍼런스)만 할당되고 실제 데이터는 힙 영역에서 할당된다.
변수를 복사하더라도 하나의 값을 가리키고 있기 때문에 복사본과 원본이 모두 같은 값을 갖는다.
변수를 복사하더라도 레퍼런스 카운트만 +1되고 실제 값이 복사되지는 않는다.
