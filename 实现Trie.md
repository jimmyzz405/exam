```java
public class Trie {
    private List<String> words;


    public Trie() {
        words = new ArrayList();
    }


    public void insert(String word) {
        words.add(word);
    }


    public boolean search(String word) {
        return words.contains(word);
    }


    public boolean startsWith(String prefix) {
        for (String word : words) {
            if (word.startsWith(prefix)) {
                return true;
            }
        }
        return false;
    }
}
```

