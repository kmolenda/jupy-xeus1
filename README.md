# jupy-lab: środowisko do ćwiczeń

* Krzysztof Molenda

Wersja przeglądarkowa JupyterLab, wykorzystująca kernel `xeus`.

Nie wymaga instalowania czegokolwiek na lokalnym komputerze. Nie wymaga też rejestracji. Kod uruchamiany jest w przeglądarce, a nie na serwerze (technologia WASM). Wersja ta jest przeznaczona do ćwiczeń i nie wymaga instalacji JupyterLab ani Pythona na lokalnym komputerze.

Wersja dostosowana jest do prowadzania moich ćwiczeń - wymagane pakiety zostały preinstalowane.

Publikowane dokumenty wykorzystują MyST Markdown, który jest rozszerzeniem Markdown. W przypadku otwarcia dokumentu w innych środowiskach niektóre treści mogą być niepoprawnie wyświetlane, ale nadal powinny być czytelne, zaś kod powinien działać poprawnie.

## Technikalia

Sprawdzenie wersji Pythona można wykonać poleceniem:

```python
import sys
print(sys.version)
```

Sprawdzenie dostępnych pakietów można wykonać poleceniem:

```python
from importlib.metadata import distributions

for dist in distributions():
    print(f"{dist.metadata['Name']}=={dist.version}")
```

