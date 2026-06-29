# 2task1
// Rectangle.java

public class Rectangle {

    private double length;
    private double width;

       public Rectangle(double length, double width) {
        this.length = length;
        this.width = width;
    }

    // Method to calculate area
    public double calculateArea() {
        return length * width;
    }

    // Method to calculate perimeter
    public double calculatePerimeter() {
        return 2 * (length + width);
    }

    // Method to display details
    public void displayDetails() {
        System.out.println("----------------------------");
        System.out.println("Length : " + length);
        System.out.println("Width  : " + width);
        System.out.println("Area   : " + calculateArea());
        System.out.println("Perimeter : " + calculatePerimeter());
    }
}

#
// Main.java

public class Main {

    public static void main(String[] args) {

        // Creating Rectangle objects
        Rectangle rectangle1 = new Rectangle(10, 5);
        Rectangle rectangle2 = new Rectangle(8, 4);
        Rectangle rectangle3 = new Rectangle(15, 7);

        // Displaying details
        System.out.println("Rectangle 1");
        rectangle1.displayDetails();

        System.out.println("\nRectangle 2");
        rectangle2.displayDetails();

        System.out.println("\nRectangle 3");
        rectangle3.displayDetails();
    }
}
