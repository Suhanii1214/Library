import java.util.Scanner;
public class Library {
    String books[];
    int no_of_books;
    Library() {
        this.books=new String[100];
        this.no_of_books=0;
    }
    void addBook(String book) {
        this.books[no_of_books]=book;
        no_of_books++;
    }
    void showAvailableBook() {
        System.out.println("Available books are:");
        for(int i=0;i<this.books.length;i++) {
            if(books[i]==null)
                continue;
           System.out.println(books[i]);
        }
    }
    void issueBook(String book) {
        for(int i=0;i<books.length;i++) {
            if(books[i]==book) {
                System.out.println(book + " has been issued!");
                this.books[i] = null;
                return;
            }
        }
        System.out.println("Book not found");
    }
    void returnBook(String book){
        addBook(book);
    }
    public static void main(String [] args) {
        Library lib=new Library();
        Scanner sc=new Scanner(System.in);
        lib.addBook("Java");
        lib.addBook("Ansi C");
        lib.addBook("Python Expert");
        lib.addBook("Harry Potter");
        lib.addBook("Hunger Games");
        lib.addBook("Scared Games");
        lib.addBook("Naughtiest Girl");
        lib.addBook("My Javascript");
        lib.addBook("Perfect Solution: C++");
        lib.addBook("My WebDev Guide");
        System.out.println("Enter the action:");
        System.out.println("Add\nIssue\nReturn\nShow");
        String str=sc.next();
        String b;
        if(str.equalsIgnoreCase("add")) {
            System.out.println("Enter the name book ");
            b=sc.next();
            System.out.println("Book added:");
            lib.addBook(b);
            System.out.println("* "+b);
        }
        else if(str.equalsIgnoreCase("issue")) {
            System.out.println("Enter the name book ");
            b=sc.next();
            lib.issueBook(b);
        }
        else if(str.equalsIgnoreCase("show")) {
            lib.showAvailableBook();
        }
        else if(str.equalsIgnoreCase("return")) {
            System.out.println("Enter the name book ");
            b=sc.next();
            lib.returnBook(b);
            System.out.println("Book return complete");
        }
    }
}
