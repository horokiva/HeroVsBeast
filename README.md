# HeroVsBeast

Tento kód řeší problém útěku hrdiny z bludiště, ve kterém se nachází pastě, zdi a nepřítel (beast). Používá Breadth-First Search (BFS) k nalezení nejkratší cesty k východu, přičemž se vyhýbá překážkám a sleduje pohyb nepřítele.

## Co kód dělá?
**1. Reprezentace mapy:** Bludiště je definováno pomocí tří typů dlaždic – prázdná, zeď, past. Hrdina (H), nepřítel (B) a východ (E) mají pevně stanovené pozice.

**2. Pohyb nepřítele:** Nepřítel se pohybuje automaticky podle definované logiky (dvakrát za tah hrdiny, může nebo nemusí šlapat na pasti).
 
**4. Hledání cesty:** Algoritmus BFS systematicky prozkoumává možné tahy hrdiny a současně sleduje pohyb nepřítele.

**5. Ověření řešení:** Kód testuje několik předpřipravených map a ověřuje, zda nalezená cesta odpovídá očekávanému výsledku.

## Použité technologie a koncepty:
- C++ (Moderní C++ - C++20):
  - STL kontejnery: `vector`, `queue`, `map`, `set`
  - Smart pointers & optional features
  - `std::optional`, `std::array`, `std::tuple`
  - Operator overloading & `std::compare` (C++20)
- Algoritmy a datové struktury:
  - Breadth-First Search (BFS) pro hledání nejkratší cesty
  - State-space search s udržováním stavu (Position hero, Position beast)
    
Jedná se o implementaci vhodnou pro AI a herní logiku, kde se sleduje pohyb dvou entit (hrdina a nepřítel) v mřížkovém světě.
