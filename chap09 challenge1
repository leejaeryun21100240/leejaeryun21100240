class EnglishScore implements Comparable<EnglishScore>{
    String name;
    int score;

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

public class EnglishTest {
    static EnglishScore findBest(EnglishScore[] a){
        EnglishScore best = a[0];

        for (int i = 0; i < a.length; i++){
            if (best.compareTo(a[i]) < 0)
                best = a[i];
        }

        return best;
    }

    public static void main(String[] args) {
        EnglishScore[] ea = {new EnglishScore("김삿갓", 77), new EnglishScore("장영실",88),new EnglishScore("홍길동", 99)};

        System.out.println("영어 최고 점수 : " + findBest(ea));
    }
}
