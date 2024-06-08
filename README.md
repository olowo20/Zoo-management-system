// Animal class
class Animal {
    String name;
    int age;

    public void makeSound() {
        // Default makeSound method
    }

    public void eat() {
        // Default eat method
    }

    public void makeSound(int times) {
        // Overloaded makeSound method
    }

    public void eat(String foodType) {
        // Overloaded eat method
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

        // Polymorphism using overloaded methods
        lion.makeSound();
        lion.eat();
        lion.makeSound(3);
        lion.eat("meat");

        elephant.makeSound();
        elephant.eat();
        elephant.makeSound(2);
        elephant.eat("grass");

        monkey.makeSound();
        monkey.eat();
        monkey.makeSound(4);
        monkey.eat("bananas");
    }
}
