import java.util.*;
public class task1{
    public static int convertFahrenheit(int temp){
    int tempc=((temp-32)*5/9);
    int tempk=((temp-32)*5/9+273);
       System.out.println("Temperature in celcius "+ tempc);
       System.out.println("Temperature in kelvin "+ tempk);
       return tempc+tempk;
    }
    public static int convertKelvin(int temp){
        int tempc=temp+273;
     int tempf=(9/5*(tempc+32));
       System.out.println("Temperature in celcius "+ tempc);
       System.out.println("Temperature in fahrenheit "+ tempf);
    return tempc+tempf;
    }
        public static int convertCelcius(int temp){
            int tempk=temp-273;
            int tempf=(temp*(9/5)+32);
            System.out.println("Temperature in kelvin "+ tempk);
            return tempk+tempf;
        }
     public static void main(String[] args) {
    Scanner sc=new Scanner(System.in);
    System.out.println("Enter thetemperature");
    int temp=sc.nextInt();
    System.out.println("Enter the unit of the temperature");
    String ch=sc.next().toUpperCase();
    switch(ch){
       case"F":    System.out.println(convertFahrenheit(temp));
       break;
       case"K":    System.out.println(convertKelvin(temp));
       break;
       case"C":    System.out.println(convertCelcius(temp));
       break;
       default:    System.out.println("Invalid");
    }
}

}
