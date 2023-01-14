# Github
 
### Utwórz bądź sklonuj istniejące repozytorium z platformy Github.
```bash
# Inicjowanie repozytorium lokalnie
git init
```

```bash
# Pobierania repozytorium z serwera zdalnego (e.g Github) 
git clone <Repository_URL>
```


---

### Upewniamy się, że jesteśmy na branch `main`/`master`
```bash
git branch --show-current
```
![git command](../PP-SDA/assets/git/git%20branch%20--show-current.png)


---

### Dla każdego `taska` / `feature'a` (zmiany w kodzie, którą będziemy wprowadzać) tworzymy nowy `branch`
```bash
git checkout -b <branch_name>
```
![git command](../PP-SDA/assets/git/git%20checkout%20-b.png)


---

### Po wprowadzeniu zmiany (zaimplementowaniu feature'a), tworzymy `commit`.
```bash
git commit -m "Commit message goes here"
```
![git commit](../PP-SDA/assets/git/git%20commit.png)


---

### Na tym etapie zawsze warto sprawdzić status zmian oraz historie commit'ów (`log`).
```bash
# Sprawdzenie statusu plików
git status
```
![git command](../PP-SDA/assets/git/git%20status.png)


---

```bash
# Sprawdzenie historii commit'ów
git log
```
![git command](../PP-SDA/assets/git/git%20log%20SS.png)

#### Note: By wyjść z logu, naciśnij klawisz `q`. 

---

### Następnie, jeżeli wszystko się zgadza wysyłamy zmiany na Github (`remota`).
```bash
git push
```

#### Potencjalne problemy to:
> - Nieustawione repozytorium zdalne:

![git command](../PP-SDA/assets/git/git%20push%20no%20repo.png)
 
> - Rozwiązanie:

![git command](../PP-SDA/assets/git/git%20add%20remote.png)

> - Nieustawiony upstream (Na jaki `origin` i `branch` wysyłać zmiany)

![git command](../PP-SDA/assets/git/git%20push%20no%20%20upstream.png)

> - Rozwiązanie:

![git command](../PP-SDA/assets/git/git%20push%20success.png)


---

> - Po wysłaniu zmian na `remota` wchodzimy na daną platformę (e.g `GitHub`) i tworzymy `Pull Request` - (`PR`)

![github ss](../PP-SDA/assets/git/gh%20PR1.png)
![github ss](../PP-SDA/assets/git/gh%20PR2.png)
![github ss](../PP-SDA/assets/git/gh%20PR3.png)

> - Prosimy kogoś o zrobienie Code Review
> - Reviewer przegląda kod i komentuje rzeczy, które są błędne lub ma co do nich wątpliwości
> - Odnosimy się do uwag reviewera, nanosimy poprawki, ew toczymy dyskusję w komentarzach
> - Gdy wszystko jest poprawione i dostajemy `Approve` od Reviewera, możemy dokonać Merge'a (guzik `Merge Pull Request`)

![github ss](../PP-SDA/assets/git/gh%20PR%20Merge.png)


---

> - Jeżeli branch nie jest nam już więcej potrzebny, klikamy `Delete Branch`

![github ss](../PP-SDA/assets/git/gh%20branch%20delete.png)


---

> - Przechodzimy na `main` / `master` i pobieramy zmiany
```bash
git checkout master
```
![git command](../PP-SDA/assets/git/git%20checkout%20master.png)


```bash
git pull
```
![git command](../PP-SDA/assets/git/git%20pull.png)

---

> - Powtarzamy proces dla każdego kolejnego feature'a
