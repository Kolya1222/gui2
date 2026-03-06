# Лабараторная работа 3

## Листинг кода для тестирования

```python
def factorial(n):
    if n < 0:
        raise ValueError("Факториал определён только для неотрицательных чисел.")
    if n == 0:
        return 1
    return n * factorial(n - 1)
```

### Код тестирования

```python
import pytest
from factorial import factorial

def test_factorial_positive():
    assert factorial(5) == 120

def test_factorial_zero():
    assert factorial(0) == 1

def test_negative_input_raises_error():
    with pytest.raises(ValueError):
        factorial(-1)

```
## Результаты тестирования

<img src="https://github.com/Kolya1222/gui2/blob/main/lr_3_test.png" alt="Тестирование Python кода">
