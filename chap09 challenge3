import java.io.IOException;
import java.security.spec.RSAOtherPrimeInfo;

class EnglishScore implements Comparable<EnglishScore>{
    String name;
    int score;
    private EnglishScore o;

    public EnglishScore(String name, int score) {
        this.name = name;
        this.score = score;
    }

    @Override
    public String toString() {
        return name + ", " + score;
    }

    @Override
    public int compareTo(EnglishScore o) {
        return score - o.score;
    }
}

class MathScore implements Comparable<MathScore>{
    String name;
    int score;

    public MathScore(String name, int score) {
        this.name = name;
        this.score = score;
    }

    @Override
    public String toString() {
        return name + ", " + score;
    }

    @Override
    public int compareTo(MathScore o) {
        return score - o.score;
    }
}

public class EnglishTest {
    static <T extends Comparable>T findBest(T[] a){
        T best = a[0];

        for (int i = 0; i < a.length; i++){
            if (best.compareTo(a[i]) < 0)
                best = a[i];
        }
        return best;
    }

    static <T>T findBest(T[] a, String name){
        for (int i = 0; i < a.length; i++){
            if (a[i].toString().substring(0, name.length()).equals(name))
                return a[i];
        }
        return null;
    }

    public static void main(String[] args) {
        EnglishScore[] ea = {new EnglishScore("김삿갓", 77), new EnglishScore("장영실",88),new EnglishScore("홍길동", 99)};
        MathScore[] ma = {new MathScore("김삿갓", 80), new MathScore("장영실",98),new MathScore("홍길동", 70)};
        String name = null;

        System.out.println("영어 최고 점수 : " + findBest(ea));
        System.out.println("수학 최고 점수 : " + findBest(ma));

        try {
            findBest(ea, name);
            findBest(ma, name);
        } catch (NullPointerException e) {
            System.out.println("명령행 인자가 없습니다.");
        } catch (Exception e){
            System.out.println("어이쿠!!!");
        }
    }
}
