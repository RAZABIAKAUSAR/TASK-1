import java.util.*;
class TEMPCONVERTER{
    public static void kelvin(int temp, String unit){
       
           float temp1=temp-273;
           float temp2=(9/5(k-273)+32);
           System.out.println("Temperature in celcius "+ temp1);
           System.out.println("Temperature in fahrenheit "+ temp2);
        }
        public static void celcius(int temp, String unit){
            
                float temp1=temp+273;
                float temp2=(9/5(temp)+32);
                System.out.println("Temperature in kelvin "+ temp1);
                System.out.println("Temperature in fahrenheit "+ temp2);
            }
            public static void fahrenheit(int temp, String unit){
            
                    float temp1=((temp-32)/1.80);
                    float temp2=(5/9(temp)+273)
                    System.out.println("Temperature in celcius "+ temp1);
                    System.out.println("Temperature in kelvin "+ temp2);
                }
    }

    public static void main(Strings args[]){
        Scanner sc=new Scanner(System.in);
        System.out println("Enter the requied temperature value");
        float temp=sc.nextInt(); String unit="K"||"C"||"F";
        if(unit!="C" && unit !="k"){
            fahrenheit();
        }
        elseif{
            if(unit!="F" && unit !="k")
            celcius();  
        }
        elseif{
            kelvin();
        }
        
}
