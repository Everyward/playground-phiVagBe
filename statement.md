# Object and Primitive Arrays

This Java template lets you get started quickly with a simple one-page playground.

```java runnable
// { autofold
import java.util.Arrays;
import java.util.stream.IntStream;
import java.util.stream.Stream;
public class Main {

public static void main(String[] args) {
// }
        //Object Array
        String[] array = {"t", "e", "c", "h", "i", "o"};

        //Arrays.stream
        Stream<String> stream1 = Arrays.stream(array);
        stream1.forEach(x -> System.out.print(x));
        System.out.println();

        //Stream.of
        Stream<String> stream2 = Stream.of(array);
        stream2.forEach(x -> System.out.print(x));
        System.out.println();
        
        //Premitive Array
         int[] intArray = {1, 2, 3, 4, 5};

        //Arrays.stream
        IntStream intStream1 = Arrays.stream(intArray);
        intStream1.forEach(x -> System.out.print(x));
        System.out.println();

        //Stream.of
        Stream<int[]> tempStream = Stream.of(intArray);
        IntStream intStream2 = tempStream.flatMapToInt(x -> Arrays.stream(x));
        intStream2.forEach(x -> System.out.print(x));
        System.out.println();

//{ autofold
}

}
//}
```

# Advanced usage

If you want a more complex example (external libraries, viewers...), use the [Advanced Java template](https://tech.io/select-repo/385)
