# oops
class Car {
    // Attributes
    String model;
    String color;

    // Constructor
    Car(String model, String color) {
        this.model = model;
        this.color = color;
    }

    // Start method
    void start() {
        if (model == null || model.isEmpty()) {
            System.out.println("Car started");
        } else {
            System.out.println("Car started");
        }
    }

    // Stop method
    void stop() {
        System.out.println("Car stopped");
    }

    // Main method for test cases
    public static void main(String[] args) {

        // TC1: Car("Tesla", "Red") → Output: Car started
        Car car1 = new Car("Tesla", "Red");
        car1.start();

        // TC2: Car("BMW", "Black") → Output: Car started
        Car car2 = new Car("BMW", "Black");
        car2.start();

        // TC3: Car model empty → Output: Car started (but model not shown)
        Car car3 = new Car("", "Blue");
        car3.start();

        // TC4: Start method not called → Output: Nothing
        Car car4 = new Car("Audi", "White");
        // No method called

        // TC5: Call stop method only → Output: Car stopped
        Car car5 = new Car("Ford", "Green");
        car5.stop();
    }
}
