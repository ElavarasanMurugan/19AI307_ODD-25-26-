# Ex.No:4(C)  COMPOSITION IN JAVA

## QUESTION:
Implement a system where a Library contains multiple Book objects. Each Book is created inside the Library. Books can't exist independently (Composition).

## AIM:
To write a Java program that demonstrates composition by creating a Library class that contains Book objects.

## ALGORITHM :

    
1. Define a class Book with private attributes title and author.
    * Provide a constructor to initialize these attributes.
    * Provide a method getDetails() to return book information.
2. Define a class Library that contains a list of Book objects.
    * Initialize the list in the constructor
    * Provide a method addBook(String title, String author) that creates a Book object and adds it to the list.
    * Provide a method showBooks() that prints all books in the library.
3. In the main method:
    * Create a Library object.
    * Read the number of books n.
    * For each book, read title and author and call addBook().
    * Finally, call showBooks() to display all books.
4. End the program.



## PROGRAM:
 ```
/*
Program to implement a Composition Concepts in Java
Developed by: Elavarasan M
RegisterNumber:  212224040083
*/
```

## SOURCE CODE:


```java
import java.util.*;

public class CompositionExample {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Library library = new Library();

        int n = sc.nextInt();
        sc.nextLine();

        for (int i = 0; i < n; i++) {
            String title = sc.nextLine();
            String author = sc.nextLine();
            library.addBook(title, author);
        }

        library.showBooks();
        sc.close();
    }
}

class Book {
    private String title;
    private String author;

    public Book(String title, String author) {
        this.title = title;
        this.author = author;
    }

    public String getDetails() {
        return title + " by " + author;
    }
}

class Library {
    private List<Book> books;

    public Library() {
        books = new ArrayList<>();
    }

    public void addBook(String title, String author) {
        Book book = new Book(title, author); // Composition: Book created inside Library
        books.add(book);
    }

    public void showBooks() {
        System.out.println("Books in Library:");
        for (Book book : books) {
            System.out.println("- " + book.getDetails());
        }
    }
}

```




## OUTPUT:

![alt text](image.png)

## RESULT:
The program successfully demonstrates composition by showing that a Library is composed of multiple Book objects.