
'Main.java'
```Java
public class Main {
	public static void main(String[] args) {

	}
	public String notString(String str) {
		return str;
	}
}
```

`MainTest.java`
```Java
import static org.junit.jupiter.api.Assertions.*;

import org.junit.jupiter.api.DisplayName;
import org.junit.jupiter.api.Test;

public class MainTest {
	private final Main main = new Main();

	@Test
	@DisplayName("1st test : true")
	void notStringTest1() {
		String str = "str";
		assertEquals(str,main.notString(str));
	}
	@Test
	@DisplayName("2st test : true")
	void notStringTest2() {
		String str = "str";
		assertEquals(str,main.notString(str));
	}
	@Test
	@DisplayName("3rd test : fail")
	void notStringTest3() {
		String str = "str";
		assertEquals("string",main.notString(str));
	}
}
```
