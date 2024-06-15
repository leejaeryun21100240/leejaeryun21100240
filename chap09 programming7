public class BoxTest {
    public static void main(String[] args) {
        Box<Integer> i = new Box<>();
        i.set(new Integer(100));
        System.out.println(i.get());

        Box<String> s = new Box<>();
        s.set("만능이네!");
        System.out.println(s.get());
    }
}

class Box<T>{
    private T obj;

    public void set(T obj) {
        this.obj = obj;
    }

    public T get() {
        return obj;
    }
}
