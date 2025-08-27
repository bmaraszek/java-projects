# How to Organize Leetcode-Style Tasks

- For the ease of testing small functions, include tests in the same file as the main code
- Follow this pattern:

```java
import org.junit.jupiter.api.DisplayName;
import org.junit.jupiter.api.Nested;
import org.junit.jupiter.api.Test;

/*
 * Explanation of the task and the approach to solve
 *
 * Time Complexity is O(N) - where N is the input size
 * Space Complexity is O(N) - where N is the input size
 */
public class NameOfTheTask {

  public static boolean isAnagram(String a, String b) {
    // implementation
  }

  @Nested
  class Tests {
    @Test
    @DisplayName("Name of the test")
    void shouldDoThisAndThat() {
      // implementation
    }
  }

}
```

- Using a nested class allows to execute all tests in one go while still placing them in the same file