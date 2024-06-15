package challenge.one;

import java.util.ArrayList;
import java.util.Iterator;
import java.util.List;

public class CapitalsDemo {
    public static void main(String[] args) {
        List<String> capitals = new ArrayList<>();
        capitals.add("서울");
        capitals.add("워싱턴");
        capitals.add("베이징");
        capitals.add("파리");
        capitals.add("마드리드");

        for (String capital : capitals)
            System.out.print(capital + " ");
        System.out.println();

        capitals.add("런던");
        Iterator<String > i = capitals.iterator();
        while(i.hasNext())
            System.out.print(i.next() + " ");
        System.out.println();

        capitals.removeIf(s -> s.length() > 2);
        capitals.forEach(s -> System.out.print(s + " "));
    }
}
