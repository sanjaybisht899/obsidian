
---
The first line in a shell script is called the **shebang (`#!`) line**, and it specifies the interpreter that should execute the script.

### **Example:**

```sh
#!/bin/bash
```

This tells the system to use the **Bash shell** to execute the script.

### **Purpose of Shebang (`#!`)**

1. **Specifies the Interpreter** – Ensures the script runs with the correct shell (e.g., Bash, Python, Perl).
2. **Avoids Manual Invocation** – Allows running the script directly (`./script.sh`) instead of using `bash script.sh`.
3. **Ensures Portability** – If the script is used on different systems, specifying `#!/usr/bin/env bash` ensures the correct interpreter is found in the environment.

### **Other Examples:**

- `#!/bin/sh` → Uses the default shell (`sh`)
- `#!/usr/bin/env python3` → Runs the script using Python 3
- `#!/usr/bin/perl` → Uses Perl interpreter
---

