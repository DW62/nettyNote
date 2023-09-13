# Headline

> An awesome project.



```css
div{
    color:red;
}
```

```java
public class TestScatteringReads {
    public static void main(String[] args) {
        try (FileChannel channel = new RandomAccessFile("word.txt", "r").getChannel()) {
            ByteBuffer b1=ByteBuffer.allocate(3);
            ByteBuffer b2=ByteBuffer.allocate(3);
            ByteBuffer b3=ByteBuffer.allocate(5);
            channel.read(new ByteBuffer[]{b1,b2,b3});
            //切换读模式
            b1.flip();
            b2.flip();
            b3.flip();
        } catch (IOException e) {
        }
    }
}
```
```php
function getAdder(int $x): int 
{
    return 123;
}
```
