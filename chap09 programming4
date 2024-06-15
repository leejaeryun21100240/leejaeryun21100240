public class PairTest {
    public static void main(String[] args) {
        Pair<Integer> p1 = new Pair<>(10,20);
        Pair<Double> p2 = new Pair<>(10.0,20.0);

        System.out.println(p1.first());
        System.out.println(p2.second());
    }
}

class Pair<T>{
    public T num1;
    public T num2;

    public Pair(T num1, T num2) {
        this.num1 = num1;
        this.num2 = num2;
    }

    T first(){
        return num1;
    }

    T second(){
        return num2;
    }
}
