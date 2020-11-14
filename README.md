# Java_shape
Choose a shape then calculate its area or perimeter based 
Specific parameters. 

package LectEnhancedBeta;
import java.util.Scanner;
public class Main {
//import main method.

    public static void main(String[] args) {
        String shape;
        int x = 0;
        boolean valu = false;
        while (x<2) {
            do {
                Scanner inShape = new Scanner(System.in);
                System.out.println("Enter your desired shape: " +
                        "Sqaure, Rectange, Circle or Triangle");
                shape = inShape.next();
            } while (!shape.equals("Square") && !shape.equals("Triangle") &&
                    !shape.equals("Circle") && !shape.equals("Rectangle"));
            if (shape.equals("Square")) {
                Scanner interCalc = new Scanner(System.in);
                System.out.println("Enter {A} for Area or {P} for Perimeter");
                String arPer = interCalc.next();
                if (arPer.equals("A")) {
                    Square.calcArea();
                } else if (arPer.equals("P")) {
                    Square.calcPerimeter();
                }
                valu = true;
                System.out.print("!");
            }
            if (shape.equals("Rectangle")) {
                Scanner interCalc = new Scanner(System.in);
                System.out.println("Enter {A} for Area or {P} for Perimeter");
                String arPer = interCalc.next();
                if (arPer.equals("A")) {
                    Rectangle.calcArea();
                } else if (arPer.equals("P")) {
                    Rectangle.calcPerimeter();
                }
                valu = true;
                System.out.print("!");
            }
            if (shape.equals("Circle")) {
                Scanner interCalc = new Scanner(System.in);
                System.out.println("Enter {A} for Area or {P} for Perimeter");
                String arPer = interCalc.next();
                if (arPer.equals("A")) {
                    Circle.calcArea();
                } else if (arPer.equals("P")) {
                    Circle.calcPerimeter();
                }
                valu = true;
                System.out.print("!");
            }
            if (shape.equals("Triangle")) {
                Scanner interCalc = new Scanner(System.in);
                System.out.println("Enter {A} for Area or {P} for Perimeter");
                String arPer = interCalc.next();
                if (arPer.equals("A")) {
                    Triangle.calcArea();
                } else if (arPer.equals("P")) {
                    Triangle.calcPerimeter();
                }
                valu = true;
                System.out.print("!");
            }
        if (valu == true){
            break;
                    }
        else if (valu == false){
           x++;
           break;
                    }
        }
    }
}


