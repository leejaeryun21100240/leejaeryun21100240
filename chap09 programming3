import java.util.NoSuchElementException;
import java.util.StringTokenizer;

public class ToeknPrintTest {
    public static void main(String[] args) {
        String s = "of the people, by the people, for the people";
        try {
            showToken(s, ", ");
        } catch (NoSuchElementException e ){
            System.out.println("끝");
        } catch (Exception e){
            System.out.println("어이쿠!!!");
        }
    }

    static void showToken(String s1, String s2){
        StringTokenizer st = new StringTokenizer(s1, s2);
        while(true){
            System.out.println(st.nextToken());
        }
    }
}
