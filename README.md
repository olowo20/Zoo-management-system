# Zoo-management-system
The Zoo class contains the main method where instances of Lion, Elephant, and Monkey are created to demonstrate polymorphism by calling the overridden methods for making sounds and eating specific foods.
 the code is as below 
 // Animal class
class Animal {
    String name;
    int age;

    public void makeSound() {
        // Default sound
    }

    public void eat() {
        // Default eating behavior
    }

    public void makeSound(int times) {
        // Overloaded method for making sound multiple times
    }

    public void eat(String foodType) {
        // Overloaded method for eating a specific food type
    }
}

// Lion class
class Lion extends Animal {
    @Override
    public void makeSound() {
        System.out.println("Roar");
    }

    @Override
    public void eat() {
        System.out.println("Eating meat");
    }
}

// Elephant class
class Elephant extends Animal {
    @Override
    public void makeSound() {
        System.out.println("Trumpet");
    }

    @Override
    public void eat() {
        System.out.println("Eating grass");
    }
}

// Monkey class
class Monkey extends Animal {
    @Override
    public void makeSound() {
        System.out.println("Chatter");
    }

    @Override
    public void eat() {
        System.out.println("Eating bananas");
    }
}

// Zoo class
public class Zoo {
    public static void main(String[] args) {
        Animal lion = new Lion();
        Animal elephant = new Elephant();
        Animal monkey = new Monkey();

        // Polymorphism demonstration
        lion.makeSound();
        lion.eat();
        elephant.makeSound();
        elephant.eat();
        monkey.makeSound();
        monkey.eat();
    }
}
