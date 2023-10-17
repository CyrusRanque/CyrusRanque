public class Book{
    private String author;
    private String title;
    private int pages;
     boolean checkout;

    public Book(String author, String title, int pages, boolean checkout){
        this.author = author;
        this.title = title;
        this.pages = pages;
        this.checkout = checkout;
    }
    public String getAuthor(){
        return author;
    }
    public String getTitle(){
        return title;
    }
    public int getPages(){
        return pages;
    }
    public boolean getCheckout() {
        return checkout;
    }


    public void setAuthor(String author){
        this.author = author;
    }
    public void setTitle(String title){
        this.title = title;
    }
    public void setPages(int pages){
        this.pages = pages;
    }
    public  void setCheckout(boolean checkout){
        this.checkout = checkout;
    }
    public void update(){
        System.out.println("Author: " + author);
        System.out.println("Checkout: " + checkout);

    }
    public void Borrowed(){
        if (checkout == true){
            System.out.println("It is being borrowed");
        }else{
            System.out.println("It is not");
        }
    }
}



