# Java-Fundamentals

Below it's some java code lessons that I studied and understand in a previous course:


![Code source](https://user-images.githubusercontent.com/114149873/199276576-e21755b0-5af1-4545-8ba3-cf74249b4864.jpg)


**Data types - Primitives – CODING:**



public class MyFirstJavaApp {

    public static void main(String[] args) {
        byte numberOfSeats = 5;
        byte numberOfDoors = 3;
        byte numberOfVehicleOwners = 1;
        byte emissionSticker = 4;

        short power = 362;
        short horsePower = 492;
        short co2Emission = 333;
        short cubicCapacity = 6417;

        int price = 29999;
        int mileage = 14999;

        long registrationNumber = 134513532145234553L;

        float fuelConsumptionCombined = 15.5F;
        float fuelConsumptionUrban = 21.4F;
        float fuelConsumptionExtraUrban = 13.6F;

        double fuelConsumptionPreciseAverage = 153.2452345234525E-1;

        boolean isDamaged = true;
        char energyEfficiencyCategory = 'G';


        System.out.println("2018 Dodge Challenger SRT 392");
        System.out.println("Price: €" + price);
        System.out.println("Mileage: " + mileage + "km");
        System.out.println("The car is damaged: " + isDamaged);
        System.out.println("Registration number: " + registrationNumber);
        System.out.println("Cubic capacity: " + cubicCapacity);
        System.out.println("Power: " + power + "kW(" + horsePower + "hp)");
        System.out.println("CO2 emission: " + co2Emission + "g/km");
        System.out.println("Emission sticker: " + emissionSticker + " ( Energy efficiency: " + energyEfficiencyCategory + ")");
        System.out.println("Combined fuel consumption: " + fuelConsumptionCombined + "l/100km");
        System.out.println("Urban fuel consumption: " + fuelConsumptionUrban + "l/100km");
        System.out.println("Extra urban fuel consumption: " + fuelConsumptionExtraUrban + "l/100km");
        System.out.println("Precise combined fuel consumption: " + fuelConsumptionPreciseAverage + "l/100km");
        System.out.println("Number of previous owners: " + numberOfVehicleOwners);
        System.out.println("Number of doors: " + numberOfDoors);
        System.out.println("Number of seats: " + numberOfSeats);

        System.out.println("Conversion");
        short newNumberOfSeats = numberOfSeats;
        System.out.println("New value of number of seats: " + newNumberOfSeats);

        int newMileage = mileage;
        System.out.println("New value of mileage: " + newMileage);

        byte newPower = (byte) power;
        System.out.println("New value of power: " + newPower);

    }
}

-------------------------------------------------

**Data types - Primitives Conversion:**



public class MyFirstJavaApp {

    public static void main(String[] args) {
        byte numberOfSeats = 5;
        byte numberOfDoors = 3;
        byte numberOfVehicleOwners = 1;
        byte emissionSticker = 4;

        short power = 362;
        short horsePower = 492;
        short co2Emission = 333;
        short cubicCapacity = 6417;

        int price = 29999;
        int mileage = 14999;

        long registrationNumber = 134513532145234553L;

        float fuelConsumptionCombined = 15.5F;
        float fuelConsumptionUrban = 21.4F;
        float fuelConsumptionExtraUrban = 13.6F;

        double fuelConsumptionPreciseAverage = 153.2452345234525E-1;

        boolean isDamaged = true;
        char energyEfficiencyCategory = 'G';


        System.out.println("2018 Dodge Challenger SRT 392");
        System.out.println("Price: €" + price);
        System.out.println("Mileage: " + mileage + "km");
        System.out.println("The car is damaged: " + isDamaged);
        System.out.println("Registration number: " + registrationNumber);
        System.out.println("Cubic capacity: " + cubicCapacity);
        System.out.println("Power: " + power + "kW(" + horsePower + "hp)");
        System.out.println("CO2 emission: " + co2Emission + "g/km");
        System.out.println("Emission sticker: " + emissionSticker + " ( Energy efficiency: " + energyEfficiencyCategory + ")");
        System.out.println("Combined fuel consumption: " + fuelConsumptionCombined + "l/100km");
        System.out.println("Urban fuel consumption: " + fuelConsumptionUrban + "l/100km");
        System.out.println("Extra urban fuel consumption: " + fuelConsumptionExtraUrban + "l/100km");
        System.out.println("Precise combined fuel consumption: " + fuelConsumptionPreciseAverage + "l/100km");
        System.out.println("Number of previous owners: " + numberOfVehicleOwners);
        System.out.println("Number of doors: " + numberOfDoors);
        System.out.println("Number of seats: " + numberOfSeats);

        System.out.println("Conversion");
        short newNumberOfSeats = numberOfSeats;
        System.out.println("New value of number of seats: " + newNumberOfSeats);

        int newMileage = mileage;
        System.out.println("New value of mileage: " + newMileage);

        byte newPower = (byte) power;
        System.out.println("New value of power: " + newPower);

    }
}

-------------------------------------------------
**Data types - Object references:**



public class ObjectReferencesApp {
    public static void main(String[] args) {
    
        Byte numberOfSeats = 5;
        Short horsePower = 392;
        Integer price = 14999;
        Long registrationNumber = 23452352345245234L;

        Float fuelConsumptionUrban = 15.5F;
        Double fuelConsumptionPreciseAverage = 15.235252345;

        Boolean isDamaged = true;
        Character energyEfficiencyCategory = 'G';

        String carType = "Dodge Challenger SRT 392";
        String carTypeWithNewKeyword = new String("Dodge Challenger SRT 392");

        System.out.println("Number of seats: " + numberOfSeats);
        System.out.println("Horsepower: " + horsePower + "hp");
        System.out.println("Price: €" + price.floatValue() );
        System.out.println("Registration number: " + registrationNumber);
        System.out.println("Urban fuel consumption: " + fuelConsumptionUrban + "l/100km");
        System.out.println("Precise average fuel consumption: " + fuelConsumptionPreciseAverage.intValue() + "l/100km");
        System.out.println("The car is damaged: " + isDamaged);
        System.out.println("Energy efficiency category: " + energyEfficiencyCategory);
        System.out.println("Car model: " + carType);
        System.out.println("Car model with uppercase: " + carType.toUpperCase());
        System.out.println("Car model with lowercase: " + carType.toLowerCase());
        System.out.println("Car model with new keyword: " + carTypeWithNewKeyword);
        System.out.println("carType variable equals to carTypeWithNewKeyword: " + carTypeWithNewKeyword.equals(carType));

        
    }
}

-----------------------
 **Operators:**



public class OperatorsApp {

    public static void main(String[] args) {

        String carModel = "Dodge Challenger SRT 392";
        int price = 14999;
        int moneyInTheBank = 100000;
        boolean isDamaged = true;

        System.out.println("Price of a " + carModel + ": €" + price);

        int increasedPrice = price + 1000;
        System.out.println("The increased price of a " + carModel + ": €" + increasedPrice);
        int decreasedPrice = price - 1000;
        System.out.println("The decreased price of a " + carModel + ": €" + decreasedPrice);
        int twoCarsPrice = price * 2;
        System.out.println("Two " + carModel + ": €" + twoCarsPrice);
        int dodgesYouCanBuy = moneyInTheBank / price;
        System.out.println("From the money we have in the bank we can buy " + dodgesYouCanBuy + " " + carModel);
        int moneyRemaining = moneyInTheBank % price;
        System.out.println("Money we would remain after buying " + dodgesYouCanBuy + " " + carModel + ": €" + moneyRemaining);
        System.out.println();

        int priceNegative = -14999;
        int priceNegativeWithPlusSign = +priceNegative;
        System.out.println("Negative price with plus sign: €" + priceNegativeWithPlusSign);
        int priceNegativeWithMinusSign = -priceNegative;
        System.out.println("Negative price with minus sign: €" + priceNegativeWithMinusSign);
        int priceOneEuroIncrease = ++price;
        System.out.println("Price after 1 euro price increase: €" + priceOneEuroIncrease);
        int priceOneEuroDecrease = --price;
        System.out.println("Price after 1 euro price decrease: €" + priceOneEuroDecrease);
        System.out.println("This car is damaged: " + !isDamaged);
        System.out.println();

        System.out.println("Car's price equals the money in the bank: " + (price == moneyInTheBank));
        System.out.println("Car's price doesn't equal the money in the bank: " + (price != moneyInTheBank));
        System.out.println("Car's price is greater than the money in the bank: " + (price > moneyInTheBank));
        System.out.println("Car's price is lesser than the money in the bank: " + (price < moneyInTheBank));
        System.out.println("Car's price is greater than or equals the money in the bank: " + (price >= moneyInTheBank));
        System.out.println("Car's price is lesser or equals than the money in the bank: " + (price <= moneyInTheBank));
        System.out.println("The carModel variable's datatype is a String: " + (carModel instanceof String));
        System.out.println();

        String damagedText = isDamaged ? "The car is damaged" : "The car isn't damaged";
        System.out.println(damagedText);
        System.out.println();

        String worthSeeingText = !isDamaged || price <= 20000 ? "It's worth seeing the car" : "It isn't worth seeing the car";
        System.out.println(worthSeeingText);
        String worthRepairingText = isDamaged && price <= 10000 ? "It's worth repairing the car" : "It isn't worth repairing the car";
        System.out.println(worthRepairingText);

        price += 1000;
        System.out.println("Price increased: €" + price);
        price -= 2000;
        System.out.println("Price decreased: €" + price);
        price *= 2;
        System.out.println("Price multiplied: €" + price);
        price /= 2;
        System.out.println("Price divided: €" + price);
        price %= 10000;
        System.out.println("Price remained: €" + price);

    }
}

-------------------------


**Loops:**



public class LoopsApp {

    public static void main(String[] args) {
        int i = 1;
        while (i <= 0){
            System.out.println(i +". BEING RIGHT SUCKS");
            i++;
        }
        System.out.println("Value of i: " + i);
        System.out.println();

        int j = 1;
        do {
            System.out.println(j +". BEING RIGHT SUCKS");
            j++;
        } while(j <= 0);
        System.out.println("Value of j: " + j);
        System.out.println();

        for (int k = 1; k<=5; k++){
            if(k ==3){
                break;
            }
            System.out.println(k +". BEING RIGHT SUCKS");
        }
        System.out.println();

        for (int k = 1; k<=5; k++){
            for (int l = 1; l<=2; l++){
                System.out.println("k=" + k + " l=" + l + " BEING RIGHT SUCKS");
            }
        }
        System.out.println();
    }
}


-------------------------------

**ControlFlowApp:**




public class ControlFlowApp {

    public static void main(String[] args) {
        boolean isDamaged = false;
        String carColor = "purple";
        char energyEfficiencyCategory = 'Z';

        if (isDamaged) {
            System.out.println("Damaged car");
        } else {
            System.out.println("Accident free car");
        }

        if (carColor.equals("red")) {
            System.out.println("This car is red");
        } else if (carColor.equals("green")) {
            System.out.println("This car is green");
        } else if (carColor.equals("blue")) {
            System.out.println("This car is blue");
        } else {
            System.out.println("I have no idea what's the color of the car");
        }

        switch (energyEfficiencyCategory) {
            case 'A':
            case 'B':
                System.out.println("Low energy consumption");
                break;
            case 'G':
                System.out.println("Very high energy consumption");
                break;
            default:
                System.out.println("Not defined category");
        }

        {
            int numberOfOwners = 5;
            {
                numberOfOwners++;
            }
            System.out.println("Number of owners: " + numberOfOwners);
        }
    }
}

--------------------------------------------------


**Methods:**




public class FunctionApp {

    public static void main(String[] args) {
        sayHello();
        blackboardPunishment(5);
        System.out.println("The price with 10% off: " + getTenPercentOffDiscountPrice(20000));
        System.out.println("The price with 50% off: " + getDiscountPrice(20000, 50));
        System.out.println("The price with 40% off: " + getDiscountPrice(20000.75, 60));
        System.out.println(getEnergyEfficiency('b'));
        getCarDescription("Tesla Roadster", 2018, "good");
    }

    static void sayHello(){
        System.out.println("Hello!!!");
    }

    static void blackboardPunishment(int repeatNumber){
        for (int i = 1; i <= repeatNumber; i++){
            System.out.println("BEING RIGHT SUCKS!");
        }
    }

    static double getTenPercentOffDiscountPrice(int price){
        return price * 0.9;
    }

    static double getDiscountPrice(int price, int percent){
        return price * percent / 100.0;
    }

    static double getDiscountPrice(double price, int percent){
        return price * percent / 100;
    }

    static String getEnergyEfficiency(char category){
        switch (category){
            case 'A':
            case 'a':
                return "Very low energy consumption";
            case 'B':
            case 'b':
                return "Low energy consumption";
            case 'C':
            case 'c':
                return "Normal energy consumption";
            case 'D':
            case 'd':
                return "Above normal energy consumption";
            case 'E':
            case 'e':
                return "High energy consumption";
            case 'F':
            case 'f':
                return "Very high energy consumption";
            case 'G':
            case 'g':
                return "Extremely high energy consumption";
            default:
                return "not defined category";
        }
    }

    static void getCarDescription(String model, int productionYear, String condition){
        System.out.println("This car is a " + model);
        System.out.println("Production year: " + productionYear);
        System.out.println("It is in " + condition + " condition");

    }
}

------------------------------------------

**Arrays:**



public class ArraysApp {

    public static void main(String[] args) {
    
        int[] lotteryNumbers = new int[5];

        lotteryNumbers[0] = 17;
        lotteryNumbers[1] = 23;
        lotteryNumbers[2] = 67;
        lotteryNumbers[3] = 37;
        lotteryNumbers[4] = 11;


        for (int lotteryNumber : lotteryNumbers){
            System.out.println(lotteryNumber);
        }

        int[][] weeklyLotteryNumbers = {
                {1, 2, 3, 4, 5},
                {10, 20, 30, 40, 50},
                {13, 24, 35, 46, 57},
                {10, 23, 35, 48, 58}
        };

        for (int i = 0; i < weeklyLotteryNumbers.length; i++) {
            for (int j = 0; j < weeklyLotteryNumbers[i].length; j++) {
                System.out.print(weeklyLotteryNumbers[i][j] + " ");
            }
            System.out.println();
        }
    }
}








