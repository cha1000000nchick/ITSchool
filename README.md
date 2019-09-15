# ITSchool


import java.util.Scanner;

  class Calculate
{
 public static void main (String[] args){
  
 Scanner in = new Scanner(System.in);
 
 
 String yesStop = "Yes";
 do {
  
 System.out.println("Введите первое число: ");
 int FirstNum = in.nextInt();
 
 System.out.println("Введите второе число: ");
 int SecondNum = in.nextInt();
 
 System.out.println("Введите знак: ");
 String Sign = in.next();
 
 switch(Sign){
  case "+":
 System.out.println( FirstNum + " + " + SecondNum + " = " + (FirstNum + SecondNum));
 break;
  case "-":
  System.out.println( FirstNum + " - " + SecondNum + " = " + (FirstNum - SecondNum));
  break;
  case "/":
  System.out.println( FirstNum + " / " + SecondNum + " = " + (FirstNum / SecondNum));
  break;
  case "*" :
  System.out.println( FirstNum + " * " + SecondNum + " = " + (FirstNum * SecondNum));
  break;
  };
 System.out.println("Хотите продолжать? (Yes/Stop)");
 yesStop = in.nextLine();
 } while (yesStop != "Stop");
  
 } 
}
