## **Glavna funkcija**

- **Java**
    
    ```java
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
    ```
    
- **Dart**
    
    ```dart
    void main() {
        print('Hello, World!');
    }
    ```
    

## **Varijable**

- **Java**
    
    ```java
    int x = 5;
    String name = "John";
    ```
    
- **Dart**
    
    ```dart
    var x = 5;
    String name = 'John';
    ```
    

## **Osnovni tipovi podataka**

### **Java**

- `int`, `float`, `double`, `char`, `boolean`
- `String`, nizovi, objekti
    
    ```java
    int broj = 10;
    double cijena = 99.99;
    boolean aktivan = true;
    String ime = "Marko";
    ```
    

### **Dart**

- `int`, `double`, `String`, `bool`
- **Korištenje `var` i `dynamic` za automatsko određivanje ili dinamičku promjenu tipa podataka**
    
    ```dart
    int broj = 10;
    double cijena = 99.99;
    bool aktivan = true;
    String ime = "Marko";
    
    var grad = "Zagreb";
    dynamic promjenjiva = 5;
    promjenjiva = "Petar";  // Tip se može mijenjati
    ```
    

## **Klase i objekti**

- **Java**
    
    ```java
    class Korisnik {
        String ime;
        Korisnik(String ime) {
            this.ime = ime;
        }
    }
    ```
    
- **Dart**
    
    ```dart
    class Korisnik {
        String ime;    
        Korisnik(this.ime);
    }
    ```
    

## **Nasljeđivanje**

- **Java**
    
    ```java
    class Admin extends Korisnik {
        Admin(String ime) {
            super(ime);
        }
    }
    ```
    
- **Dart**
    
    ```dart
    class Admin extends Korisnik {
        Admin(String ime) : super(ime);
    }
    ```
    

## **Polimorfizam**

- **Java**
    
    ```java
    class Animal {
        void makeSound() {
            System.out.println("Animal sound");
        }
    }
    class Dog extends Animal {
        void makeSound() {
            System.out.println("Bark");
        }
    }
    ```
    
- **Dart**
    
    ```dart
    class Animal {
        void makeSound() {
            print('Animal sound');
        }
    }
    class Dog extends Animal {
        void makeSound() {
            print('Bark');
        }
    }
    ```
    

## **Funkcije**

- **Java**
    
    ```java
    void pozdrav() {
        System.out.println("Pozdrav!");
    }
    ```
    
- **Dart**
    
    ```dart
    void pozdrav() {
        print('Pozdrav!');
    }
    ```
    

## **Petlje**

- **Java**
    
    ```java
    for (int i = 0; i < 5; i++) {
        System.out.println(i);
    }
    ```
    
- **Dart**
    
    ```dart
    for (var i = 0; i < 5; i++) {
        print(i);
    }
    ```
    

## **Kontrolne strukture**

- **Java**
    
    ```java
    if (x > 5) {
        System.out.println("Greater");
    } else {
        System.out.println("Smaller");
    }
    ```
    
- **Dart**
    
    ```dart
    if (x > 5) {
        print('Greater');
    } else {
        print('Smaller');
    }
    ```
    

## Upravljanje iznimkama

- **Java**
    
    ```java
    try {
        // code
    } catch (Exception e) {
        // handle exception
    }
    ```
    
- **Dart**
    
    ```dart
    try {
        // code
    } catch (e) {
        // handle exception
    }
    ```
    

## Skupine podataka

### **Java**

U **Java** jeziku, postoje različite vrste kolekcija, koje dolaze iz **Java Collections Framework-a**. Najčešće korištene kolekcije uključuju:

- **Arrays**: Fiksne veličine, mogu pohranjivati primitivne tipove ili objekte.
    - Primjer: `int[] brojevi = new int[5];`
- **ArrayList**: Dinamička lista koja može mijenjati veličinu.
    - Primjer: `ArrayList<String> imena = new ArrayList<>();`
- **LinkedList**: Implementira listu koristeći povezane čvorove. Dobro za operacije umetanja i brisanja.
    - Primjer: `LinkedList<Integer> brojevi = new LinkedList<>();`
- **HashSet**: Kolekcija koja ne dopušta duplikate i ne osigurava redoslijed.
    - Primjer: `HashSet<String> set = new HashSet<>();`
- **HashMap**: Struktura ključ-vrijednost, gdje svaki ključ mora biti jedinstven.
    - Primjer: `HashMap<Integer, String> mapa = new HashMap<>();`

### **Dart**

U **Dart** jeziku, najčešće korištene kolekcije su:

- **List**: Dinamičke ili fiksne duljine, može pohranjivati bilo koji tip podataka.
    - Primjer: `List<int> brojevi = [1, 2, 3];`
- **Set**: Kolekcija koja ne dopušta duplikate i automatski uklanja višak istih elemenata.
    - Primjer: `Set<String> set = {'Ana', 'Marko', 'Ana'};` // Ispisuje samo {'Ana', 'Marko'}
- **Map**: Struktura ključ-vrijednost, gdje svaki ključ mora biti jedinstven.
    - Primjer: `Map<int, String> mapa = {1: 'Ana', 2: 'Marko'};`

### **Usporedba Java i Dart kolekcija**

| Kolekcija | **Java** | **Dart** |
| --- | --- | --- |
| **Lista (List)** | `ArrayList`, `LinkedList` | `List` (fiksna ili dinamična) |
| **Skup (Set)** | `HashSet`, `TreeSet` | `Set` (dinamična kolekcija) |
| **Mapa (Map)** | `HashMap`, `TreeMap` | `Map` (dinamična struktura) |
| **Niz (Array)** | `int[]`, `String[]` | `List.filled` (fiksna duljina) |

## **Asinkrono programiranje**

### **Java**

- **`CompletableFuture`**: Asinkrono programiranje pomoću `CompletableFuture` za izvršavanje zadataka u pozadini i obradu rezultata nakon završetka.
    
    ```java
    import java.util.concurrent.CompletableFuture;
    
    public class AsyncExample {
        public static void main(String[] args) {
            CompletableFuture<Void> future = CompletableFuture.runAsync(() -> {
                try {
                    Thread.sleep(2000);
                    System.out.println("Zadatak završen");
                } catch (InterruptedException e) {
                    e.printStackTrace();
                }
            });
    
            System.out.println("Glavna nit nastavlja dalje...");
            future.join();  // Čeka završetak asinkronog zadatka
        }
    }
    ```
    

### **Dart**

- **`async/await`**: Dart koristi ključne riječi `async` i `await` za asinkrone funkcije koje vraćaju `Future`. `await` omogućuje čekanje na asinkroni rezultat bez blokiranja glavnog toka.
    
    ```dart
    void main() async {
      print("Pokretanje asinkronog zadatka...");
      await longRunningTask();
      print("Zadatak završen, nastavljamo dalje.");
    }
    
    Future<void> longRunningTask() async {
      await Future.delayed(Duration(seconds: 2));
      print("Asinkroni zadatak izvršen.");
    }
    ```
    

**Ključne razlike u asinkronom programiranju**:

- **Java** koristi `CompletableFuture`, što je vrlo moćno i fleksibilno, ali složenije za rad.
- **Dart** koristi jednostavan `async/await` model koji omogućava čitljiviji i prirodniji kod.