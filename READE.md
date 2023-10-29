https://github.com/{username}/{repository}/raw/{branch}/{path_to_file}

https://github.com/hougarry/FreecodeCamp-Notes/raw/main/avatar.jpg

https://github.com/hougarry/Image-hosting-service/raw/main/avatar/profile.png
To use the raw path in your code, you can use the following code:

```python
import requests # pip install requests

url = "" # raw path
r = requests.get(url)
print(r.text)
```

```javascript
fetch('https://raw.githubusercontent.com/{username}/{repository}/{branch}/{path_to_file}')
  .then(response => response.text())
  .then(data => console.log(data))
```

```html
<img src="https://raw.githubusercontent.com/{username}/{repository}/{branch}/{path_to_file}" alt="alt text" title="Title" />
```

```css
body {
  background: url(https://raw.githubusercontent.com/{username}/{repository}/{branch}/{path_to_file});
}

```java
import java.io.IOException;
import java.net.URL;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) throws IOException {
        URL url = new URL("https://raw.githubusercontent.com/{username}/{repository}/{branch}/{path_to_file}");
        Scanner scanner = new Scanner(url.openStream());
        while (scanner.hasNext()) {
            System.out.println(scanner.nextLine());
        }
    }
}
```
