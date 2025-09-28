## 🔐 Random Password Generator (Python)

This simple Python script generates a secure random password using a combination of:
- Uppercase and lowercase letters  
- Digits  
- Special characters  

### 📜 Code
```python
import random
import string

def generate_password(length: int = 10):
    alphabet = string.ascii_letters + string.digits + string.punctuation
    password = ''.join(random.choice(alphabet) for i in range(length))
    return password

password = generate_password()
print(f"Generated password: {password}")
