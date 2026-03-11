# 📚 OOP, SOLID Principles & Design Patterns — Interview Q&A

> **Bilingual (English / Tiếng Việt) | Java Code Examples | Senior Developer Level**
>
> A comprehensive guide covering 46 interview questions across three major categories.

---

## 📋 Table of Contents

### Part 1: Object-Oriented Programming (OOP)
- [Q1. What are the four pillars of OOP?](#q1-what-are-the-four-pillars-of-object-oriented-programming-oop)
- [Q2. Difference between abstraction and encapsulation](#q2-explain-the-difference-between-abstraction-and-encapsulation)
- [Q3. What is polymorphism in Java?](#q3-what-is-polymorphism-and-how-is-it-implemented-in-java)
- [Q4. How does inheritance work?](#q4-how-does-inheritance-work-in-oop-what-are-its-benefits-and-drawbacks)
- [Q5. Method overloading vs method overriding](#q5-what-is-the-difference-between-method-overloading-and-method-overriding)
- [Q6. Interface vs abstract class](#q6-what-is-an-interface-in-java-and-how-is-it-different-from-an-abstract-class)
- [Q7. Access modifiers in Java](#q7-how-do-access-modifiers-public-private-protected-default-work-in-java)
- [Q8. Class vs object](#q8-what-is-the-difference-between-a-class-and-an-object)
- [Q9. Constructors in Java](#q9-what-are-constructors-in-java-and-how-do-they-work)
- [Q10. Deep copy vs shallow copy](#q10-what-is-the-difference-between-deep-copy-and-shallow-copy)
- [Q11. Static methods and variables](#q11-what-are-static-methods-and-static-variables-when-should-they-be-used)
- [Q12. final vs finally vs finalize](#q12-what-is-the-difference-between-final-finally-and-finalize-in-java)
- [Q13. Enums in Java](#q13-what-is-an-enum-in-java-and-when-should-it-be-used)
- [Q14. Java memory management and GC](#q14-how-does-java-handle-memory-management-and-garbage-collection)
- [Q15. equals() vs ==](#q15-what-is-the-equals-method-in-java-and-how-is-it-different-from-)
- [Q16. Java Beans and POJOs](#q16-what-are-java-beans-and-pojos-how-are-they-used)
- [Q17. The toString() method](#q17-what-is-the-role-of-the-tostring-method-in-java)
- [Q18. Singleton class implementation](#q18-what-is-a-singleton-class-and-how-can-it-be-implemented)
- [Q19. The hashCode() method](#q19-what-is-the-hashcode-method-in-java-and-why-is-it-important)
- [Q20. Mutable vs immutable objects](#q20-what-is-the-difference-between-a-mutable-and-an-immutable-object)

### Part 2: SOLID Principles and Clean Code
- [Q21. What are the SOLID principles?](#q21-what-are-the-solid-principles-and-why-are-they-important)
- [Q22. Single Responsibility Principle (SRP)](#q22-explain-the-single-responsibility-principle-srp-with-an-example)
- [Q23. Open/Closed Principle (OCP)](#q23-what-is-the-openclosed-principle-ocp-and-how-does-it-improve-code-maintainability)
- [Q24. Liskov Substitution Principle (LSP)](#q24-how-does-the-liskov-substitution-principle-lsp-prevent-design-issues)
- [Q25. Interface Segregation Principle (ISP)](#q25-what-is-the-interface-segregation-principle-isp-and-when-should-it-be-applied)
- [Q26. Dependency Inversion Principle (DIP)](#q26-explain-the-dependency-inversion-principle-dip-with-a-real-world-example)
- [Q27. Best practices for clean code](#q27-what-are-the-best-practices-for-writing-clean-and-maintainable-code)
- [Q28. Code smells](#q28-how-do-code-smells-impact-software-maintainability)
- [Q29. Refactoring techniques](#q29-what-are-some-common-refactoring-techniques-to-improve-code-quality)
- [Q30. Cyclomatic complexity](#q30-what-is-cyclomatic-complexity-and-why-is-it-important-in-software-development)
- [Q31. Enforcing coding conventions](#q31-how-do-you-enforce-coding-conventions-in-a-large-development-team)
- [Q32. Common anti-patterns](#q32-what-are-some-common-anti-patterns-in-software-development)
- [Q33. DRY vs WET](#q33-what-is-the-difference-between-dry-dont-repeat-yourself-and-wet-write-everything-twice)
- [Q34. Exception handling in Java](#q34-how-do-you-handle-exceptions-properly-in-java)
- [Q35. Law of Demeter](#q35-what-is-the-law-of-demeter-and-why-should-it-be-followed)
- [Q36. Test-Driven Development (TDD)](#q36-what-is-test-driven-development-tdd-and-how-does-it-improve-code-quality)
- [Q37. Logging in Java applications](#q37-how-do-you-use-logging-effectively-in-a-java-application)
- [Q38. Self-documenting code](#q38-what-is-the-benefit-of-writing-self-documenting-code)
- [Q39. Dependency injection in Java](#q39-how-do-you-implement-dependency-injection-in-java)
- [Q40. Modular and reusable code](#q40-what-are-some-best-practices-for-designing-modular-and-reusable-code)

### Part 3: Design Patterns
- [Q41. What are design patterns?](#q41-what-are-design-patterns-and-why-are-they-useful)
- [Q42. Factory pattern](#q42-explain-the-factory-pattern-and-provide-an-example)
- [Q43. Singleton pattern](#q43-how-does-the-singleton-pattern-work-and-what-are-its-pros-and-cons)
- [Q44. Adapter vs Bridge pattern](#q44-what-is-the-difference-between-the-adapter-and-bridge-design-patterns)
- [Q45. Observer pattern](#q45-how-does-the-observer-pattern-work-and-where-is-it-commonly-used)
- [Q46. Strategy pattern](#q46-what-is-the-strategy-pattern-and-how-does-it-help-with-code-flexibility)

---
# 🧱 PART 1: Object-Oriented Programming (OOP)

---
## Q1. What are the four pillars of Object-Oriented Programming (OOP)?

### 🇬🇧 English

Object-Oriented Programming is built upon four fundamental pillars: **Encapsulation**, **Inheritance**, **Polymorphism**, and **Abstraction**. These concepts together allow developers to model real-world entities in code, promote reuse, and build maintainable systems.

#### 1. Encapsulation
Bundling data (fields) and behavior (methods) into a single unit (class), and restricting direct access to some components. It's like a capsule that protects the data inside.

#### 2. Inheritance
The mechanism by which a class (child) can acquire properties and behaviors from another class (parent). Think of how a `Dog` is-a `Animal`.

#### 3. Polymorphism
The ability of an object to take many forms. A `Shape` reference can point to a `Circle`, `Rectangle`, or `Triangle` — each behaving differently when calling `draw()`.

#### 4. Abstraction
Hiding complex implementation details and showing only the necessary interface. Like driving a car — you use the steering wheel without knowing how the engine works.

```java
// ============================================================
// Demonstrating all four OOP pillars with a Shape hierarchy
// ============================================================

// ABSTRACTION: Abstract class hides implementation details
abstract class Shape {
    private String color;  // ENCAPSULATION: private field

    public Shape(String color) {
        this.color = color;
    }

    // Getter - controlled access (Encapsulation)
    public String getColor() {
        return color;
    }

    // Abstract method - forces subclasses to implement (Abstraction)
    public abstract double area();

    // Concrete method available to all subclasses (Inheritance)
    public void displayInfo() {
        System.out.println("Shape: " + getClass().getSimpleName()
            + ", Color: " + color
            + ", Area: " + String.format("%.2f", area()));
    }
}

// INHERITANCE: Circle inherits from Shape
class Circle extends Shape {
    private double radius;

    public Circle(String color, double radius) {
        super(color);  // Call parent constructor
        this.radius = radius;
    }

    // POLYMORPHISM: overriding parent's abstract method
    @Override
    public double area() {
        return Math.PI * radius * radius;
    }
}

// INHERITANCE: Rectangle inherits from Shape
class Rectangle extends Shape {
    private double width;
    private double height;

    public Rectangle(String color, double width, double height) {
        super(color);
        this.width = width;
        this.height = height;
    }

    @Override
    public double area() {
        return width * height;
    }
}

// INHERITANCE: Triangle inherits from Shape
class Triangle extends Shape {
    private double base;
    private double height;

    public Triangle(String color, double base, double height) {
        super(color);
        this.base = base;
        this.height = height;
    }

    @Override
    public double area() {
        return 0.5 * base * height;
    }
}

// Demo
public class OOPPillarsDemo {
    public static void main(String[] args) {
        // POLYMORPHISM: Shape reference pointing to different subtypes
        Shape[] shapes = {
            new Circle("Red", 5.0),
            new Rectangle("Blue", 4.0, 6.0),
            new Triangle("Green", 3.0, 8.0)
        };

        // Each shape behaves differently - runtime polymorphism
        for (Shape shape : shapes) {
            shape.displayInfo();
        }
        // Output:
        // Shape: Circle, Color: Red, Area: 78.54
        // Shape: Rectangle, Color: Blue, Area: 24.00
        // Shape: Triangle, Color: Green, Area: 12.00
    }
}
```

**When to use OOP:**
- Modeling real-world entities (User, Order, Product)
- Building large-scale applications that require maintainability
- When you want reusable and extensible code

**Common Mistakes:**
- Over-engineering with deep inheritance hierarchies (prefer composition)
- Breaking encapsulation by exposing mutable internal state

---

### 🇻🇳 Tiếng Việt

Lập trình hướng đối tượng (OOP) xây dựng trên bốn trụ cột chính: **Đóng gói**, **Kế thừa**, **Đa hình**, và **Trừu tượng hóa**.

#### 1. Đóng gói (Encapsulation)
Gói dữ liệu và hành vi vào một đơn vị (class) và kiểm soát quyền truy cập. Giống như một viên nang bảo vệ dữ liệu bên trong. Dùng `private` cho fields, `public` cho getters/setters.

#### 2. Kế thừa (Inheritance)
Cơ chế cho phép một class con nhận các thuộc tính và phương thức từ class cha. `Dog` kế thừa từ `Animal` — chó là một loại động vật.

#### 3. Đa hình (Polymorphism)
Khả năng một đối tượng có thể biểu hiện dưới nhiều hình thức. Cùng một lời gọi `shape.area()` nhưng kết quả khác nhau tùy theo loại hình.

#### 4. Trừu tượng hóa (Abstraction)
Ẩn đi sự phức tạp, chỉ phơi bày những gì cần thiết. Giống lái xe — bạn dùng vô lăng mà không cần biết cách động cơ hoạt động.

**Lỗi thường gặp:**
- Tạo cây kế thừa quá sâu → khó bảo trì
- Làm vỡ đóng gói bằng cách return trực tiếp mutable object bên trong

---
## Q2. Explain the difference between abstraction and encapsulation.

### 🇬🇧 English

Though often confused, abstraction and encapsulation address different concerns:

| Aspect | Abstraction | Encapsulation |
|--------|-------------|---------------|
| **Purpose** | Hide complexity, show only essentials | Bundle data + behavior, restrict access |
| **Focus** | *What* an object does | *How* it protects its data |
| **Achieved via** | Abstract classes, interfaces | Access modifiers (private, protected) |
| **Design level** | Design/architecture level | Implementation level |
| **Analogy** | TV remote (you press buttons, don't see electronics) | Medicine capsule (ingredients are hidden inside) |

**Abstraction** answers: "What can this object do?"
**Encapsulation** answers: "How does this object protect its state?"

```java
// ============================================================
// Abstraction vs Encapsulation — Bank Account Example
// ============================================================

// ABSTRACTION: Defines what operations a bank account supports
// Users know they can deposit, withdraw, check balance — not HOW
interface BankAccount {
    void deposit(double amount);
    boolean withdraw(double amount);
    double getBalance();
    String getAccountSummary();
}

// ENCAPSULATION: Hides the internal state and protects it
// All fields are private; validation logic is internal
class SavingsAccount implements BankAccount {
    // ENCAPSULATION: fields are private
    private final String accountNumber;
    private final String ownerName;
    private double balance;
    private double interestRate;
    private int transactionCount;

    public SavingsAccount(String accountNumber, String ownerName,
                          double initialBalance, double interestRate) {
        this.accountNumber = accountNumber;
        this.ownerName = ownerName;
        this.balance = initialBalance;
        this.interestRate = interestRate;
        this.transactionCount = 0;
    }

    // ABSTRACTION: caller doesn't need to know HOW deposit works internally
    @Override
    public void deposit(double amount) {
        if (amount <= 0) {
            throw new IllegalArgumentException("Deposit amount must be positive");
        }
        balance += amount;
        transactionCount++;
        System.out.printf("Deposited: $%.2f | New Balance: $%.2f%n", amount, balance);
    }

    // ENCAPSULATION: internal business rules are hidden from caller
    @Override
    public boolean withdraw(double amount) {
        if (amount <= 0) {
            throw new IllegalArgumentException("Withdrawal amount must be positive");
        }
        // Internal rule: maintain minimum balance of $100
        if (balance - amount < 100.0) {
            System.out.println("Insufficient funds — minimum balance required: $100");
            return false;
        }
        balance -= amount;
        transactionCount++;
        System.out.printf("Withdrawn: $%.2f | New Balance: $%.2f%n", amount, balance);
        return true;
    }

    @Override
    public double getBalance() {
        return balance;
    }

    // ENCAPSULATION: computed property — internal logic hidden
    public double calculateInterest() {
        return balance * interestRate / 100;
    }

    @Override
    public String getAccountSummary() {
        return String.format("Account: %s | Owner: %s | Balance: $%.2f | Transactions: %d",
            accountNumber, ownerName, balance, transactionCount);
    }
}

// ABSTRACTION: Another implementation — caller uses same interface
class CheckingAccount implements BankAccount {
    private String accountNumber;
    private double balance;
    private double overdraftLimit;  // Checking accounts have overdraft

    public CheckingAccount(String accountNumber, double balance, double overdraftLimit) {
        this.accountNumber = accountNumber;
        this.balance = balance;
        this.overdraftLimit = overdraftLimit;
    }

    @Override
    public void deposit(double amount) {
        balance += amount;
    }

    @Override
    public boolean withdraw(double amount) {
        // Different internal rule — allows overdraft
        if (balance - amount < -overdraftLimit) {
            System.out.println("Overdraft limit exceeded");
            return false;
        }
        balance -= amount;
        return true;
    }

    @Override
    public double getBalance() { return balance; }

    @Override
    public String getAccountSummary() {
        return String.format("Checking Account: %s | Balance: $%.2f", accountNumber, balance);
    }
}

public class AbstractionEncapsulationDemo {
    public static void main(String[] args) {
        // Abstraction in action: we use BankAccount interface
        // We don't know (or care) which implementation is used
        BankAccount account = new SavingsAccount("SA-001", "Alice", 1000.0, 3.5);
        account.deposit(500.0);
        account.withdraw(200.0);
        System.out.println(account.getAccountSummary());

        // Switching implementation without changing client code
        BankAccount checking = new CheckingAccount("CA-001", 500.0, 200.0);
        checking.withdraw(600.0);  // Uses overdraft, different internal logic
        System.out.println(checking.getAccountSummary());
    }
}
```

**Key Takeaway:**
- Abstraction is about *design* — what interface to expose
- Encapsulation is about *implementation* — how to protect data
- They work together: abstraction defines the contract; encapsulation enforces it

### 🇻🇳 Tiếng Việt

Mặc dù hay bị nhầm lẫn, hai khái niệm này giải quyết vấn đề khác nhau:

**Trừu tượng hóa (Abstraction):**
- Trả lời câu hỏi: "Đối tượng này có thể làm gì?"
- Ẩn đi sự phức tạp, chỉ phơi bày interface cần thiết
- Thực hiện qua: abstract class, interface
- Ví dụ: Remote TV — bạn chỉ thấy nút bấm, không thấy mạch điện

**Đóng gói (Encapsulation):**
- Trả lời câu hỏi: "Đối tượng bảo vệ dữ liệu như thế nào?"
- Gói dữ liệu + hành vi, kiểm soát quyền truy cập
- Thực hiện qua: access modifiers (private, protected, public)
- Ví dụ: Viên nang thuốc — thành phần bên trong được bảo vệ

**Kết hợp cả hai:** Interface `BankAccount` định nghĩa trừu tượng hóa (giao diện chung). Class `SavingsAccount` thực hiện đóng gói (ẩn `balance`, `transactionCount`, quy tắc rút tiền tối thiểu).

---
## Q3. What is polymorphism, and how is it implemented in Java?

### 🇬🇧 English

**Polymorphism** (from Greek: "many forms") allows objects of different types to be treated through a common interface, with each type behaving in its own specific way.

Java supports two types of polymorphism:

| Type | Also Called | Resolved At | Mechanism |
|------|-------------|-------------|-----------|
| **Compile-time** | Static / Method Overloading | Compile time | Same method name, different parameters |
| **Runtime** | Dynamic / Method Overriding | Runtime | Subclass overrides parent method |

```java
// ============================================================
// Polymorphism — Complete Example
// ============================================================

// --- 1. COMPILE-TIME POLYMORPHISM (Method Overloading) ---
class MathUtils {
    // Same method name, different parameter types/counts
    public int add(int a, int b) {
        return a + b;
    }

    public double add(double a, double b) {
        return a + b;
    }

    public int add(int a, int b, int c) {
        return a + b + c;
    }

    public String add(String a, String b) {
        return a + b;  // String concatenation
    }
}

// --- 2. RUNTIME POLYMORPHISM (Method Overriding) ---
abstract class Animal {
    protected String name;

    public Animal(String name) {
        this.name = name;
    }

    // This method will be overridden by each subclass
    public abstract String makeSound();

    public void describe() {
        System.out.println(name + " says: " + makeSound());
    }
}

class Dog extends Animal {
    public Dog(String name) { super(name); }

    @Override
    public String makeSound() {
        return "Woof! Woof!";
    }

    // Dog-specific behavior
    public void fetch() {
        System.out.println(name + " fetches the ball!");
    }
}

class Cat extends Animal {
    public Cat(String name) { super(name); }

    @Override
    public String makeSound() {
        return "Meow~";
    }
}

class Duck extends Animal {
    public Duck(String name) { super(name); }

    @Override
    public String makeSound() {
        return "Quack! Quack!";
    }
}

// --- 3. INTERFACE POLYMORPHISM ---
interface Drawable {
    void draw();
    default String getType() { return "Unknown Shape"; }
}

interface Resizable {
    void resize(double factor);
}

// A class can implement multiple interfaces
class Circle2D implements Drawable, Resizable {
    private double radius;

    public Circle2D(double radius) { this.radius = radius; }

    @Override
    public void draw() {
        System.out.printf("Drawing Circle with radius %.2f%n", radius);
    }

    @Override
    public void resize(double factor) {
        radius *= factor;
        System.out.printf("Circle resized — new radius: %.2f%n", radius);
    }

    @Override
    public String getType() { return "Circle"; }
}

class Square2D implements Drawable, Resizable {
    private double side;

    public Square2D(double side) { this.side = side; }

    @Override
    public void draw() {
        System.out.printf("Drawing Square with side %.2f%n", side);
    }

    @Override
    public void resize(double factor) {
        side *= factor;
    }

    @Override
    public String getType() { return "Square"; }
}

public class PolymorphismDemo {
    public static void main(String[] args) {
        // Compile-time polymorphism
        MathUtils math = new MathUtils();
        System.out.println(math.add(2, 3));          // 5
        System.out.println(math.add(2.5, 3.5));      // 6.0
        System.out.println(math.add(1, 2, 3));       // 6
        System.out.println(math.add("Hello", " World")); // Hello World

        // Runtime polymorphism — single interface, multiple behaviors
        Animal[] animals = {
            new Dog("Rex"),
            new Cat("Whiskers"),
            new Duck("Donald")
        };

        System.out.println("\n--- Animal Sounds ---");
        for (Animal animal : animals) {
            animal.describe();  // Each behaves differently
        }

        // instanceof check before downcasting
        for (Animal animal : animals) {
            if (animal instanceof Dog dog) {  // Java 16+ pattern matching
                dog.fetch();  // Access Dog-specific method safely
            }
        }

        // Interface polymorphism
        System.out.println("\n--- Drawing Shapes ---");
        Drawable[] drawables = {new Circle2D(5.0), new Square2D(4.0)};
        for (Drawable d : drawables) {
            d.draw();
            System.out.println("Type: " + d.getType());
        }
    }
}
```

**Pros of Polymorphism:**
- Code is extensible — add new types without changing existing code
- Reduces conditional logic (`if/else` chains)
- Enables dependency injection and testing with mocks

**Common Mistakes:**
- Downcasting without `instanceof` check → ClassCastException
- Confusing overloading and overriding

### 🇻🇳 Tiếng Việt

**Đa hình (Polymorphism)** là khả năng một đối tượng có thể biểu hiện dưới nhiều hình thức khác nhau. Java hỗ trợ hai loại:

**1. Đa hình tĩnh (Compile-time):** Nạp chồng phương thức (Method Overloading) — cùng tên phương thức, khác tham số. Xác định tại thời điểm biên dịch.

**2. Đa hình động (Runtime):** Ghi đè phương thức (Method Overriding) — lớp con định nghĩa lại phương thức của lớp cha. Xác định tại thời điểm chạy.

Ví dụ thực tế: Trong vòng lặp `for (Animal animal : animals)`, Java sẽ tự động gọi đúng phiên bản `makeSound()` của từng lớp con — đây chính là đa hình động.

**Lỗi thường gặp:**
- Ép kiểu (downcast) không kiểm tra `instanceof` → lỗi `ClassCastException`
- Nhầm giữa overloading và overriding

---
## Q4. How does inheritance work in OOP? What are its benefits and drawbacks?

### 🇬🇧 English

**Inheritance** is a mechanism where a child class (subclass) acquires properties and methods from a parent class (superclass), establishing an **is-a** relationship.

Java uses `extends` for class inheritance and `implements` for interface inheritance. Java supports **single inheritance** for classes (to avoid the diamond problem) but **multiple inheritance** through interfaces.

```java
// ============================================================
// Inheritance — Vehicle Hierarchy Example
// ============================================================

// Base class (Superclass)
public class Vehicle {
    private String make;
    private String model;
    private int year;
    protected double fuelLevel;  // protected: accessible in subclasses

    public Vehicle(String make, String model, int year) {
        this.make = make;
        this.model = model;
        this.year = year;
        this.fuelLevel = 100.0;
    }

    public void startEngine() {
        System.out.println(getDescription() + " engine started.");
    }

    public void stopEngine() {
        System.out.println(getDescription() + " engine stopped.");
    }

    public String getDescription() {
        return year + " " + make + " " + model;
    }

    // Getters
    public String getMake() { return make; }
    public String getModel() { return model; }
    public int getYear() { return year; }
}

// Subclass 1 — inherits from Vehicle
public class Car extends Vehicle {
    private int numberOfDoors;
    private String transmissionType;

    public Car(String make, String model, int year,
               int doors, String transmission) {
        super(make, model, year);  // Must call parent constructor
        this.numberOfDoors = doors;
        this.transmissionType = transmission;
    }

    // Overriding parent method to provide specific behavior
    @Override
    public void startEngine() {
        System.out.println("Inserting key and turning ignition...");
        super.startEngine();  // Reuse parent logic
    }

    // Car-specific method
    public void openTrunk() {
        System.out.println(getDescription() + ": Trunk opened.");
    }

    @Override
    public String getDescription() {
        return super.getDescription() + " (Car, " + numberOfDoors + " doors, " + transmissionType + ")";
    }
}

// Subclass 2
public class Truck extends Vehicle {
    private double payloadCapacityTons;
    private boolean hasTowPackage;

    public Truck(String make, String model, int year,
                 double payload, boolean towPackage) {
        super(make, model, year);
        this.payloadCapacityTons = payload;
        this.hasTowPackage = towPackage;
    }

    @Override
    public void startEngine() {
        System.out.println("Climbing into cab...");
        super.startEngine();
    }

    public void loadCargo(double weightTons) {
        if (weightTons > payloadCapacityTons) {
            System.out.printf("Warning! Overloaded by %.1f tons!%n",
                weightTons - payloadCapacityTons);
        } else {
            System.out.printf("Loaded %.1f tons (capacity: %.1f tons)%n",
                weightTons, payloadCapacityTons);
        }
    }

    @Override
    public String getDescription() {
        return super.getDescription() + " (Truck, payload: " + payloadCapacityTons + "t)";
    }
}

// Subclass 3 — multilevel inheritance
public class ElectricCar extends Car {
    private double batteryCapacityKwh;
    private int rangeKm;

    public ElectricCar(String make, String model, int year,
                       int doors, double battery, int range) {
        super(make, model, year, doors, "Automatic");
        this.batteryCapacityKwh = battery;
        this.rangeKm = range;
    }

    // Different engine start for electric car
    @Override
    public void startEngine() {
        // Don't call super — electric cars have different startup
        System.out.println(getDescription() + ": Silent electric motor engaged. Ready.");
        fuelLevel = 100.0;  // Represents battery level
    }

    public void chargeBattery() {
        System.out.printf("Charging %.1f kWh battery... Range: %d km%n",
            batteryCapacityKwh, rangeKm);
    }
}

public class InheritanceDemo {
    public static void main(String[] args) {
        Vehicle[] fleet = {
            new Car("Toyota", "Camry", 2023, 4, "CVT"),
            new Truck("Ford", "F-150", 2022, 1.5, true),
            new ElectricCar("Tesla", "Model 3", 2024, 4, 82.0, 560)
        };

        for (Vehicle v : fleet) {
            System.out.println("\n" + v.getDescription());
            v.startEngine();

            // Downcast to access subclass-specific methods
            if (v instanceof Truck truck) {
                truck.loadCargo(1.2);
            }
            if (v instanceof ElectricCar ev) {
                ev.chargeBattery();
            }
            v.stopEngine();
        }
    }
}
```

**Benefits of Inheritance:**
- ✅ Code reuse — avoid duplicating common logic
- ✅ Establishes clear type hierarchy
- ✅ Runtime polymorphism through method overriding
- ✅ Easier maintenance — fix in parent, propagates to children

**Drawbacks of Inheritance:**
- ❌ **Tight coupling** — child is tightly bound to parent
- ❌ **Fragile base class** problem — changing parent breaks children
- ❌ Deep hierarchies become hard to understand
- ❌ Java restricts to single inheritance (classes)

> **Best Practice:** Favor **composition over inheritance** for flexibility. Use inheritance only when a true **is-a** relationship exists.

```java
// Composition over Inheritance example
// Bad: ElectricEngine extends GasEngine
// Good: Car HAS-A Engine (composition)
class Engine {
    private String type;
    private int horsePower;

    public Engine(String type, int hp) {
        this.type = type;
        this.horsePower = hp;
    }

    public void start() {
        System.out.println(type + " engine (" + horsePower + "hp) started");
    }
}

class ModernCar {
    private Engine engine;  // Composition: HAS-A relationship
    private String model;

    public ModernCar(String model, Engine engine) {
        this.model = model;
        this.engine = engine;
    }

    public void start() {
        engine.start();  // Delegate to engine
        System.out.println(model + " ready to go.");
    }
}
```

### 🇻🇳 Tiếng Việt

**Kế thừa (Inheritance)** là cơ chế cho phép lớp con (subclass) nhận các thuộc tính và phương thức từ lớp cha (superclass), tạo ra mối quan hệ **is-a** (là-một).

Java dùng từ khóa `extends` cho kế thừa class, `implements` cho interface. Java chỉ hỗ trợ **đơn kế thừa** (single inheritance) với class để tránh "diamond problem", nhưng **đa kế thừa** vẫn có thể thực hiện qua interface.

**Lợi ích:**
- Tái sử dụng code — không cần viết lại logic chung
- Xây dựng hệ thống phân cấp rõ ràng
- Hỗ trợ đa hình (polymorphism)

**Nhược điểm:**
- Coupling chặt giữa lớp cha và con
- Thay đổi lớp cha có thể phá vỡ lớp con ("Fragile Base Class")
- Cây kế thừa sâu → khó hiểu, khó test

**Nguyên tắc vàng:** Ưu tiên **Composition over Inheritance** (Kết hợp thay vì Kế thừa) để tăng tính linh hoạt. Chỉ dùng kế thừa khi có quan hệ **is-a** rõ ràng (Chó là Động vật, Xe điện là Xe hơi).

---
## Q5. What is the difference between method overloading and method overriding?

### 🇬🇧 English

| Feature | Method Overloading | Method Overriding |
|---------|-------------------|-------------------|
| **Definition** | Same name, different parameters | Subclass redefines parent method |
| **Type** | Compile-time polymorphism | Runtime polymorphism |
| **Inheritance** | Not required | Required |
| **Return type** | Can differ (if parameter differs) | Must be same or covariant |
| **Access modifier** | Can differ freely | Cannot be more restrictive |
| **static/final** | Can overload these | Cannot override static/final |
| **Annotation** | No `@Override` needed | `@Override` recommended |

```java
// ============================================================
// Overloading vs Overriding — Complete Example
// ============================================================

// --- OVERLOADING: Multiple versions of same method in same class ---
class Printer {

    // Overloaded print methods — same name, different signatures
    public void print(String text) {
        System.out.println("Printing text: " + text);
    }

    public void print(int number) {
        System.out.println("Printing number: " + number);
    }

    public void print(String text, int copies) {
        for (int i = 0; i < copies; i++) {
            System.out.println("Copy " + (i+1) + ": " + text);
        }
    }

    public void print(double value, String format) {
        System.out.printf("Printing formatted: " + format + "%n", value);
    }
}

// --- OVERRIDING: Subclass provides its own implementation ---
class BaseLogger {
    protected String prefix;

    public BaseLogger(String prefix) {
        this.prefix = prefix;
    }

    public void log(String message) {
        System.out.println("[" + prefix + "] " + message);
    }

    public void logError(String message) {
        System.err.println("[ERROR][" + prefix + "] " + message);
    }

    // final method — cannot be overridden
    public final void logSystemInfo() {
        System.out.println("System: Java " + System.getProperty("java.version"));
    }
}

class FileLogger extends BaseLogger {
    private String fileName;

    public FileLogger(String prefix, String fileName) {
        super(prefix);
        this.fileName = fileName;
    }

    // OVERRIDING: Different implementation for file logging
    @Override
    public void log(String message) {
        // Widening access: parent is 'public', we keep 'public' ✓
        System.out.println("[FILE:" + fileName + "][" + prefix + "] " + message);
        // In reality, would write to file
    }

    // Can also OVERLOAD in subclass
    public void log(String message, boolean urgent) {
        if (urgent) {
            System.out.println("🚨 URGENT [FILE:" + fileName + "] " + message);
        } else {
            log(message);  // Calls the overridden method
        }
    }
}

class CloudLogger extends BaseLogger {
    private String endpoint;

    public CloudLogger(String prefix, String endpoint) {
        super(prefix);
        this.endpoint = endpoint;
    }

    @Override
    public void log(String message) {
        System.out.println("[CLOUD:" + endpoint + "] " + prefix + " > " + message);
        // In reality, would send HTTP request to log service
    }
}

public class OverloadingOverridingDemo {
    public static void main(String[] args) {
        // OVERLOADING — resolved at compile time
        Printer printer = new Printer();
        printer.print("Hello");           // calls print(String)
        printer.print(42);               // calls print(int)
        printer.print("Test", 3);        // calls print(String, int)
        printer.print(3.14, "Pi: %.4f"); // calls print(double, String)

        System.out.println();

        // OVERRIDING — resolved at runtime
        BaseLogger[] loggers = {
            new BaseLogger("APP"),
            new FileLogger("APP", "app.log"),
            new CloudLogger("APP", "logs.example.com")
        };

        for (BaseLogger logger : loggers) {
            logger.log("User logged in");  // Each calls its own version
        }

        // FileLogger also has overloaded log method
        FileLogger fileLogger = new FileLogger("SEC", "security.log");
        fileLogger.log("Suspicious activity detected", true);  // Overloaded
        fileLogger.log("Normal activity");                       // Overridden
    }
}
```

**Key Distinction:**
- Overloading is a *convenience feature* — same conceptual operation for different input types
- Overriding is about *behavioral specialization* — subtype provides its own specific behavior

**Common Mistakes:**
```java
class Parent {
    public void show(int x) { System.out.println("Parent: " + x); }
}

class Child extends Parent {
    // This is OVERLOADING, not OVERRIDING! (different parameter type)
    public void show(double x) { System.out.println("Child: " + x); }

    // This IS overriding (same signature)
    @Override
    public void show(int x) { System.out.println("Child override: " + x); }
}
```

### 🇻🇳 Tiếng Việt

**Nạp chồng (Overloading) — đa hình tĩnh:**
- Nhiều phương thức cùng tên trong cùng một class, khác nhau về tham số (số lượng, kiểu dữ liệu)
- Xác định lúc **biên dịch** (compile-time)
- Không cần kế thừa
- Ví dụ: `print(String)`, `print(int)`, `print(String, int)`

**Ghi đè (Overriding) — đa hình động:**
- Lớp con định nghĩa lại phương thức của lớp cha
- Xác định lúc **chạy** (runtime)
- Cần kế thừa
- Dùng `@Override` annotation để tránh lỗi
- Không được thu hẹp access modifier (ví dụ: không thể override `public` thành `private`)

**Quy tắc quan trọng cho Overriding:**
- Return type phải giống hoặc là subtype (covariant return type)
- Access modifier không được chặt hơn cha
- Không thể override `static`, `final`, `private` methods

---
## Q6. What is an interface in Java, and how is it different from an abstract class?

### 🇬🇧 English

Both interfaces and abstract classes enable abstraction, but they serve different purposes and have distinct rules.

| Feature | Interface | Abstract Class |
|---------|-----------|----------------|
| **Keyword** | `interface` | `abstract class` |
| **Instantiation** | Cannot instantiate | Cannot instantiate |
| **Methods** | abstract, default, static (Java 8+) | abstract + concrete |
| **Fields** | `public static final` only | Any type of fields |
| **Multiple** | A class can implement many | Only single inheritance |
| **Constructors** | No constructors | Can have constructors |
| **Access modifiers** | Methods `public` by default | Any access modifier |
| **State** | Stateless (no instance vars) | Can hold state |
| **Use case** | Define a contract/capability | Shared base implementation |

```java
// ============================================================
// Interface vs Abstract Class — Payment Processing System
// ============================================================

// INTERFACE: Defines a contract — "what can you do?"
// No state, no constructors
interface Payable {
    // Implicitly public abstract
    boolean processPayment(double amount, String currency);
    boolean refund(String transactionId, double amount);

    // Default method (Java 8+) — optional to override
    default String generateReceiptId() {
        return "RCP-" + System.currentTimeMillis();
    }

    // Static utility method
    static boolean isValidAmount(double amount) {
        return amount > 0 && amount < 1_000_000;
    }
}

// Another interface — Java classes can implement multiple interfaces
interface Auditable {
    void logTransaction(String action, double amount);
    String getAuditTrail();
}

// ABSTRACT CLASS: Provides shared implementation + forces subclass contract
// Has state, constructors, mix of abstract and concrete methods
abstract class BasePaymentProcessor implements Payable, Auditable {
    // State — abstract classes CAN have instance variables
    protected String processorName;
    protected String merchantId;
    private StringBuilder auditLog = new StringBuilder();

    // Constructor — abstract classes CAN have constructors
    public BasePaymentProcessor(String processorName, String merchantId) {
        this.processorName = processorName;
        this.merchantId = merchantId;
    }

    // Concrete method — shared by all subclasses
    protected void validatePayment(double amount, String currency) {
        if (!Payable.isValidAmount(amount)) {
            throw new IllegalArgumentException("Invalid amount: " + amount);
        }
        if (currency == null || currency.isBlank()) {
            throw new IllegalArgumentException("Currency cannot be blank");
        }
    }

    // Concrete implementation of Auditable
    @Override
    public void logTransaction(String action, double amount) {
        String entry = String.format("[%s] %s: $%.2f%n",
            processorName, action, amount);
        auditLog.append(entry);
        System.out.print(entry);
    }

    @Override
    public String getAuditTrail() {
        return auditLog.toString();
    }

    // Abstract method — subclasses MUST implement
    protected abstract String getPaymentType();

    @Override
    public String toString() {
        return processorName + " (" + getPaymentType() + ") [Merchant: " + merchantId + "]";
    }
}

// Concrete implementation 1: Credit Card
class CreditCardProcessor extends BasePaymentProcessor {
    private String cardNetwork;  // VISA, Mastercard, etc.

    public CreditCardProcessor(String merchantId, String cardNetwork) {
        super("CreditCard-" + cardNetwork, merchantId);
        this.cardNetwork = cardNetwork;
    }

    @Override
    public boolean processPayment(double amount, String currency) {
        validatePayment(amount, currency);
        // Simulate credit card processing
        System.out.printf("Processing %s card payment: $%.2f %s%n",
            cardNetwork, amount, currency);
        logTransaction("CREDIT_CHARGE", amount);
        return true;  // Assume success
    }

    @Override
    public boolean refund(String transactionId, double amount) {
        System.out.printf("Refunding credit card transaction %s: $%.2f%n",
            transactionId, amount);
        logTransaction("CREDIT_REFUND", amount);
        return true;
    }

    @Override
    protected String getPaymentType() {
        return "Credit Card (" + cardNetwork + ")";
    }
}

// Concrete implementation 2: PayPal
class PayPalProcessor extends BasePaymentProcessor {
    private String paypalEmail;

    public PayPalProcessor(String merchantId, String paypalEmail) {
        super("PayPal", merchantId);
        this.paypalEmail = paypalEmail;
    }

    @Override
    public boolean processPayment(double amount, String currency) {
        validatePayment(amount, currency);
        System.out.printf("PayPal payment from %s: $%.2f %s%n",
            paypalEmail, amount, currency);
        logTransaction("PAYPAL_CHARGE", amount);
        return true;
    }

    @Override
    public boolean refund(String transactionId, double amount) {
        System.out.printf("PayPal refund to %s for txn %s: $%.2f%n",
            paypalEmail, transactionId, amount);
        logTransaction("PAYPAL_REFUND", amount);
        return true;
    }

    // Override the default method from interface
    @Override
    public String generateReceiptId() {
        return "PP-" + System.currentTimeMillis();
    }

    @Override
    protected String getPaymentType() { return "PayPal"; }
}

// A class implementing interface directly (no abstract class needed)
class CryptoProcessor implements Payable {
    private String walletAddress;

    public CryptoProcessor(String walletAddress) {
        this.walletAddress = walletAddress;
    }

    @Override
    public boolean processPayment(double amount, String currency) {
        System.out.printf("Crypto payment to %s: %.8f BTC%n",
            walletAddress, amount / 45000); // mock BTC conversion
        return true;
    }

    @Override
    public boolean refund(String transactionId, double amount) {
        System.out.println("Crypto refunds require manual processing: " + transactionId);
        return false;
    }
}

public class InterfaceVsAbstractDemo {
    public static void main(String[] args) {
        // Using abstract class reference
        BasePaymentProcessor processor1 = new CreditCardProcessor("MERCH-001", "VISA");
        BasePaymentProcessor processor2 = new PayPalProcessor("MERCH-001", "user@email.com");

        processor1.processPayment(99.99, "USD");
        processor2.processPayment(49.50, "USD");

        // Using interface reference — includes CryptoProcessor
        Payable[] allProcessors = {processor1, processor2, new CryptoProcessor("1A2B3C")};
        for (Payable p : allProcessors) {
            p.processPayment(100.0, "USD");
        }

        // Audit trail (only available on BasePaymentProcessor subclasses)
        System.out.println("\nAudit Trail:");
        System.out.println(processor1.getAuditTrail());
    }
}
```

**When to use Interface:**
- Define a contract (capability) that unrelated classes share
- When you need multiple inheritance
- API design — define behavior without any implementation

**When to use Abstract Class:**
- Share common code among related classes
- Provide default behavior that can be overridden
- When you want to control constructor logic
- Template Method pattern

### 🇻🇳 Tiếng Việt

**Interface (Giao diện):**
- Định nghĩa hợp đồng (contract) — "đối tượng có thể làm gì?"
- Không có trạng thái (không có instance fields)
- Một class có thể `implements` nhiều interface
- Phù hợp khi muốn định nghĩa khả năng cho các class không liên quan nhau
- Từ Java 8: có thể có `default` và `static` methods

**Abstract Class (Lớp trừu tượng):**
- Cung cấp triển khai chung cho các class liên quan
- Có thể có instance fields, constructors
- Một class chỉ `extends` được một abstract class
- Phù hợp khi có code chung cần chia sẻ
- Dùng Template Method Pattern

**Khi nào dùng cái nào?**
- Dùng **Interface** khi thiết kế API, muốn nhiều class không liên quan chia sẻ behavior
- Dùng **Abstract Class** khi có nhiều class liên quan và cần chia sẻ code chung

---
## Q7. How do access modifiers (public, private, protected, default) work in Java?

### 🇬🇧 English

Access modifiers control the **visibility** and **accessibility** of classes, methods, and fields.

| Modifier | Same Class | Same Package | Subclass | Everywhere |
|----------|-----------|--------------|---------|------------|
| `public` | ✅ | ✅ | ✅ | ✅ |
| `protected` | ✅ | ✅ | ✅ | ❌ |
| `default` (no keyword) | ✅ | ✅ | ❌ | ❌ |
| `private` | ✅ | ❌ | ❌ | ❌ |

```java
// ============================================================
// Access Modifiers — Practical Example
// ============================================================
package com.example.bank;

public class BankAccount {
    // private: only accessible within BankAccount class
    private double balance;
    private String pin;

    // default (package-private): accessible within com.example.bank package
    String accountNumber;

    // protected: accessible within package + subclasses outside package
    protected String ownerName;

    // public: accessible everywhere
    public String bankName;

    public BankAccount(String owner, String pin, double initialBalance) {
        this.ownerName = owner;
        this.pin = pin;
        this.balance = initialBalance;
        this.accountNumber = generateAccountNumber();
        this.bankName = "National Bank";
    }

    // private method — internal utility only
    private String generateAccountNumber() {
        return "ACC" + (int)(Math.random() * 1_000_000);
    }

    // private — only used internally for validation
    private boolean validatePin(String inputPin) {
        return this.pin.equals(inputPin);
    }

    // public — controlled access to private field
    public double getBalance(String pin) {
        if (!validatePin(pin)) {
            throw new SecurityException("Invalid PIN");
        }
        return balance;
    }

    // public — exposed business operation
    public boolean deposit(double amount) {
        if (amount <= 0) return false;
        balance += amount;
        return true;
    }

    // protected — subclasses can override internal transfer logic
    protected boolean transferInternal(double amount) {
        if (amount > balance) return false;
        balance -= amount;
        return true;
    }

    // public API
    public boolean transfer(BankAccount target, double amount, String pin) {
        if (!validatePin(pin)) throw new SecurityException("Invalid PIN");
        if (transferInternal(amount)) {
            target.deposit(amount);
            return true;
        }
        return false;
    }
}

// Subclass in a DIFFERENT package
// Can access: public and protected members
// Cannot access: private and default members
package com.example.premium;

import com.example.bank.BankAccount;

public class PremiumAccount extends BankAccount {
    private double creditLimit;

    public PremiumAccount(String owner, String pin,
                          double balance, double creditLimit) {
        super(owner, pin, balance);
        this.creditLimit = creditLimit;
        // Can access: ownerName (protected), bankName (public)
        // Cannot access: balance (private), pin (private), accountNumber (default)
        System.out.println("Premium account created for: " + ownerName); // protected ✓
    }

    @Override
    protected boolean transferInternal(double amount) {
        // Override protected method — premium accounts can use credit
        double effectiveBalance = getBalance("0000") + creditLimit; // simplified
        return amount <= effectiveBalance;
    }
}
```

**Best Practices:**
1. **Start with most restrictive** (`private`) and open up only as needed
2. Fields should almost always be `private` — use getters/setters
3. Helper methods should be `private`
4. `protected` is appropriate for methods meant for subclasses to override
5. Avoid `default` (package-private) for public APIs — it creates implicit package coupling

```java
// Good practice — Immutable Value Object with proper access control
public final class Money {
    private final double amount;   // private, immutable
    private final String currency; // private, immutable

    public Money(double amount, String currency) {
        if (amount < 0) throw new IllegalArgumentException("Amount cannot be negative");
        this.amount = amount;
        this.currency = currency;
    }

    // Public read-only accessors
    public double getAmount() { return amount; }
    public String getCurrency() { return currency; }

    public Money add(Money other) {
        if (!this.currency.equals(other.currency)) {
            throw new IllegalArgumentException("Currency mismatch");
        }
        return new Money(this.amount + other.amount, this.currency);
    }

    @Override
    public String toString() {
        return String.format("%.2f %s", amount, currency);
    }
}
```

### 🇻🇳 Tiếng Việt

Access modifiers kiểm soát phạm vi truy cập trong Java:

- **`private`**: Chỉ trong cùng class — bảo vệ chặt nhất. Dùng cho tất cả fields.
- **`default`** (không từ khóa): Trong cùng package. Dùng cho internal helper classes.
- **`protected`**: Trong package + subclass kể cả khác package. Dùng cho method mà subclass cần override.
- **`public`**: Truy cập từ mọi nơi. Dùng cho API public.

**Nguyên tắc:** Luôn bắt đầu với phạm vi **hẹp nhất** (`private`) và chỉ mở rộng khi cần. Điều này bảo vệ dữ liệu nội bộ và giảm coupling giữa các class.

**Lỗi phổ biến:** Để fields là `public` hoặc `protected` thay vì `private`. Điều này phá vỡ đóng gói (encapsulation) — bất kỳ code nào cũng có thể thay đổi trạng thái của object.

---
## Q8. What is the difference between a class and an object?

### 🇬🇧 English

| Aspect | Class | Object |
|--------|-------|--------|
| **Definition** | Blueprint/template | Instance of a class |
| **Memory** | Loaded once (class metadata) | Each instance uses heap memory |
| **Creation** | Written by programmer | Created with `new` keyword |
| **Type** | Type definition | Concrete entity |
| **Analogy** | House blueprint | Actual house built from blueprint |
| **Count** | One per class definition | Many instances possible |

```java
// ============================================================
// Class vs Object — Student Management Example
// ============================================================

// CLASS: Blueprint for Student objects
// Defines structure and behavior, no memory allocated for data yet
public class Student {
    // Class-level metadata (static — shared across ALL instances)
    private static int totalStudents = 0;
    private static final String INSTITUTION = "Tech University";

    // Instance fields (each object has its own copy)
    private final int studentId;
    private String name;
    private double gpa;
    private List<String> enrolledCourses;

    // Constructor — creates an OBJECT (instance) from the class blueprint
    public Student(String name, double gpa) {
        this.studentId = ++totalStudents;  // Assign unique ID
        this.name = name;
        this.gpa = gpa;
        this.enrolledCourses = new ArrayList<>();
    }

    public void enroll(String course) {
        enrolledCourses.add(course);
        System.out.printf("%s enrolled in %s%n", name, course);
    }

    public String getAcademicStanding() {
        if (gpa >= 3.7) return "Honors";
        if (gpa >= 3.0) return "Good Standing";
        if (gpa >= 2.0) return "Satisfactory";
        return "Academic Probation";
    }

    // Static method — belongs to the CLASS, not any specific object
    public static int getTotalStudents() { return totalStudents; }
    public static String getInstitution() { return INSTITUTION; }

    @Override
    public String toString() {
        return String.format("Student{id=%d, name='%s', gpa=%.2f, standing='%s', courses=%s}",
            studentId, name, gpa, getAcademicStanding(), enrolledCourses);
    }

    // Getters and setters
    public int getStudentId() { return studentId; }
    public String getName() { return name; }
    public double getGpa() { return gpa; }
    public void setGpa(double gpa) { this.gpa = gpa; }
}

public class ClassVsObjectDemo {
    public static void main(String[] args) {
        // Class-level info — no instance needed
        System.out.println("Institution: " + Student.getInstitution());
        System.out.println("Students so far: " + Student.getTotalStudents()); // 0

        // Creating OBJECTS (instances) from the Student CLASS blueprint
        Student alice = new Student("Alice Johnson", 3.8);   // Object 1
        Student bob = new Student("Bob Smith", 3.1);         // Object 2
        Student carol = new Student("Carol White", 2.5);     // Object 3

        // Each object has independent state
        alice.enroll("Algorithms");
        alice.enroll("Machine Learning");
        bob.enroll("Database Systems");
        carol.enroll("Web Development");

        // Each object reports its own state
        System.out.println(alice);  // Alice's data
        System.out.println(bob);    // Bob's data
        System.out.println(carol);  // Carol's data

        // Class-level counter updated by all instances
        System.out.println("Total students: " + Student.getTotalStudents()); // 3

        // Objects are independent — modifying one doesn't affect others
        alice.setGpa(3.9);
        System.out.println("Alice GPA updated: " + alice.getGpa()); // 3.9
        System.out.println("Bob GPA unchanged: " + bob.getGpa());   // 3.1

        // Reference vs Object
        Student ref1 = alice;          // ref1 and alice point to SAME object
        Student copy = new Student("Alice Johnson", 3.9); // Completely NEW object

        System.out.println("Same object? " + (ref1 == alice));   // true
        System.out.println("Same object? " + (copy == alice));   // false
    }
}
```

**Object Identity vs Equality:**
```java
String s1 = "Hello";
String s2 = "Hello";
String s3 = new String("Hello");

System.out.println(s1 == s2);      // true (same String pool object)
System.out.println(s1 == s3);      // false (different objects in memory)
System.out.println(s1.equals(s3)); // true (same content)
```

### 🇻🇳 Tiếng Việt

**Class (Lớp)** là bản thiết kế (blueprint) — định nghĩa cấu trúc và hành vi. Giống như bản vẽ kỹ thuật của một ngôi nhà.

**Object (Đối tượng)** là thực thể cụ thể được tạo từ class — mỗi đối tượng có trạng thái riêng. Giống như ngôi nhà thực sự được xây từ bản vẽ.

- Một class có thể tạo ra **nhiều object** khác nhau
- Mỗi object có **bộ nhớ riêng** cho các instance fields
- Các `static` field/method thuộc về **class**, không phải object cụ thể
- Tạo object bằng từ khóa `new`

**Bộ nhớ:** Class metadata được nạp một lần vào **Method Area**. Mỗi object được cấp phát trong **Heap memory**.

---
## Q9. What are constructors in Java, and how do they work?

### 🇬🇧 English

A **constructor** is a special method that initializes a new object. It has the same name as the class and no return type.

**Types of Constructors:**
1. **Default constructor** — no parameters, provided by Java if none defined
2. **Parameterized constructor** — accepts arguments to initialize fields
3. **Copy constructor** — creates a new object as a copy of an existing one

```java
// ============================================================
// Constructors — Comprehensive Example
// ============================================================

public class Employee {
    private final int id;
    private String name;
    private String department;
    private double salary;
    private String email;
    private static int nextId = 1;

    // 1. PARAMETERIZED CONSTRUCTOR — Main constructor
    public Employee(String name, String department, double salary) {
        this.id = nextId++;
        this.name = validateName(name);
        this.department = department;
        this.salary = validateSalary(salary);
        this.email = generateEmail(name);
    }

    // 2. CONSTRUCTOR CHAINING with this() — reuse constructor logic
    // "Quick" constructor with just name
    public Employee(String name) {
        this(name, "General", 50_000.0);  // Delegates to main constructor
    }

    // Constructor with name and department (uses default salary)
    public Employee(String name, String department) {
        this(name, department, 50_000.0);  // Constructor chaining
    }

    // 3. COPY CONSTRUCTOR — creates a deep copy
    public Employee(Employee other) {
        this.id = nextId++;  // New unique ID
        this.name = other.name;
        this.department = other.department;
        this.salary = other.salary;
        this.email = other.email;
    }

    // Private validation methods used in constructors
    private String validateName(String name) {
        if (name == null || name.isBlank()) {
            throw new IllegalArgumentException("Name cannot be empty");
        }
        return name.trim();
    }

    private double validateSalary(double salary) {
        if (salary < 0) {
            throw new IllegalArgumentException("Salary cannot be negative");
        }
        return salary;
    }

    private String generateEmail(String name) {
        return name.toLowerCase().replace(" ", ".") + "@company.com";
    }

    // Getters
    public int getId() { return id; }
    public String getName() { return name; }
    public String getDepartment() { return department; }
    public double getSalary() { return salary; }
    public String getEmail() { return email; }

    @Override
    public String toString() {
        return String.format("Employee{id=%d, name='%s', dept='%s', salary=%.0f, email='%s'}",
            id, name, department, salary, email);
    }
}

// BUILDER PATTERN — alternative to telescoping constructors
// Use when a class has many optional parameters
public class PersonBuilder {
    // Required parameters
    private final String firstName;
    private final String lastName;

    // Optional parameters with defaults
    private int age = 0;
    private String email = "";
    private String phone = "";
    private String address = "";

    // Private constructor — force use of builder
    private PersonBuilder(Builder builder) {
        this.firstName = builder.firstName;
        this.lastName = builder.lastName;
        this.age = builder.age;
        this.email = builder.email;
        this.phone = builder.phone;
        this.address = builder.address;
    }

    public String getFullName() { return firstName + " " + lastName; }
    public int getAge() { return age; }

    // Static nested Builder class
    public static class Builder {
        private final String firstName;
        private final String lastName;
        private int age;
        private String email = "";
        private String phone = "";
        private String address = "";

        // Builder constructor requires mandatory fields
        public Builder(String firstName, String lastName) {
            this.firstName = firstName;
            this.lastName = lastName;
        }

        // Fluent setters — return Builder for chaining
        public Builder age(int age) { this.age = age; return this; }
        public Builder email(String email) { this.email = email; return this; }
        public Builder phone(String phone) { this.phone = phone; return this; }
        public Builder address(String address) { this.address = address; return this; }

        // Terminal method — creates the object
        public PersonBuilder build() {
            return new PersonBuilder(this);
        }
    }

    @Override
    public String toString() {
        return String.format("Person{name='%s %s', age=%d, email='%s'}",
            firstName, lastName, age, email);
    }
}

public class ConstructorDemo {
    public static void main(String[] args) {
        // Various constructors
        Employee emp1 = new Employee("Alice Johnson", "Engineering", 95_000);
        Employee emp2 = new Employee("Bob Smith");               // Default dept + salary
        Employee emp3 = new Employee("Carol White", "Marketing"); // Default salary
        Employee emp4 = new Employee(emp1);                       // Copy constructor

        System.out.println(emp1);
        System.out.println(emp2);
        System.out.println(emp3);
        System.out.println(emp4);  // New ID, same data as emp1

        // Builder pattern — readable for complex objects
        PersonBuilder person = new PersonBuilder.Builder("John", "Doe")
            .age(30)
            .email("john.doe@example.com")
            .phone("+1-555-1234")
            .address("123 Main St, Springfield")
            .build();
        System.out.println(person);
    }
}
```

**Constructor Rules:**
- Same name as class, no return type
- If you define no constructor, Java provides a default (no-arg) one
- If you define ANY constructor, Java will NOT provide the default
- `this()` — call another constructor in same class (must be first statement)
- `super()` — call parent constructor (must be first statement)
- You cannot call both `this()` and `super()` in same constructor

### 🇻🇳 Tiếng Việt

**Constructor (Hàm khởi tạo)** là phương thức đặc biệt được gọi khi tạo object bằng `new`. Nó không có kiểu trả về và có cùng tên với class.

**Các loại Constructor:**
1. **Default constructor**: Không tham số. Java tự cung cấp nếu bạn không định nghĩa constructor nào.
2. **Parameterized constructor**: Nhận tham số để khởi tạo fields.
3. **Copy constructor**: Tạo bản sao của object khác.

**Constructor chaining:** Dùng `this(...)` để gọi constructor khác trong cùng class — tránh lặp code. Dùng `super(...)` để gọi constructor của class cha.

**Builder Pattern:** Khi class có quá nhiều tham số tùy chọn, nên dùng Builder Pattern thay vì nhiều constructor chồng chất — code dễ đọc và an toàn hơn.

**Quy tắc quan trọng:**
- `this()` hoặc `super()` phải là câu lệnh đầu tiên trong constructor
- Không thể gọi cả `this()` và `super()` trong cùng một constructor

---
## Q10. What is the difference between deep copy and shallow copy?

### 🇬🇧 English

When copying objects, the behavior depends on how references to nested objects are handled.

| Aspect | Shallow Copy | Deep Copy |
|--------|-------------|-----------|
| **Primitive fields** | Copied by value | Copied by value |
| **Reference fields** | Copied by reference (shared) | New copies of objects created |
| **Independence** | Changes to nested objects affect both | Completely independent copies |
| **Memory** | Less memory | More memory |
| **Performance** | Faster | Slower |
| **Method** | `Object.clone()` default, copy constructor | Custom clone, serialization |

```java
// ============================================================
// Deep Copy vs Shallow Copy
// ============================================================

import java.util.ArrayList;
import java.util.List;

// Address — a mutable nested object
class Address {
    private String street;
    private String city;
    private String country;

    public Address(String street, String city, String country) {
        this.street = street;
        this.city = city;
        this.country = country;
    }

    // Copy constructor for deep copy
    public Address(Address other) {
        this.street = other.street;
        this.city = other.city;
        this.country = other.country;
    }

    public String getStreet() { return street; }
    public void setStreet(String street) { this.street = street; }
    public String getCity() { return city; }
    public void setCity(String city) { this.city = city; }

    @Override
    public String toString() {
        return street + ", " + city + ", " + country;
    }
}

// Person contains a mutable Address and a List of courses
class Person implements Cloneable {
    private String name;           // String is immutable — safe to share
    private int age;               // Primitive — always copied by value
    private Address address;       // Mutable reference object
    private List<String> hobbies;  // Mutable list

    public Person(String name, int age, Address address, List<String> hobbies) {
        this.name = name;
        this.age = age;
        this.address = address;
        this.hobbies = hobbies;
    }

    // SHALLOW COPY via clone() — default behavior
    // Primitive + String fields are safe, but Address and List are SHARED
    @Override
    public Person clone() {
        try {
            return (Person) super.clone();  // Shallow copy
        } catch (CloneNotSupportedException e) {
            throw new RuntimeException(e);
        }
    }

    // DEEP COPY — creates completely independent object
    public Person deepCopy() {
        Address newAddress = new Address(this.address);        // Copy address
        List<String> newHobbies = new ArrayList<>(this.hobbies); // Copy list
        return new Person(this.name, this.age, newAddress, newHobbies);
    }

    // Getters and setters
    public String getName() { return name; }
    public int getAge() { return age; }
    public Address getAddress() { return address; }
    public List<String> getHobbies() { return hobbies; }
    public void setName(String name) { this.name = name; }
    public void setAge(int age) { this.age = age; }

    @Override
    public String toString() {
        return String.format("Person{name='%s', age=%d, address='%s', hobbies=%s}",
            name, age, address, hobbies);
    }
}

public class CopyDemo {
    public static void main(String[] args) {
        // Original object
        Address addr = new Address("123 Main St", "Springfield", "USA");
        List<String> hobbies = new ArrayList<>();
        hobbies.add("Reading");
        hobbies.add("Coding");

        Person original = new Person("Alice", 30, addr, hobbies);
        System.out.println("Original:      " + original);

        // SHALLOW COPY
        Person shallow = original.clone();
        System.out.println("Shallow copy:  " + shallow);

        // Modify nested objects of shallow copy
        shallow.getAddress().setCity("Shelbyville"); // AFFECTS ORIGINAL!
        shallow.getHobbies().add("Gaming");          // AFFECTS ORIGINAL!
        shallow.setAge(31);                          // Does NOT affect original (primitive)
        shallow.setName("Alice (Shallow)");          // Does NOT affect original (String)

        System.out.println("\nAfter modifying shallow copy's city and hobbies:");
        System.out.println("Original:      " + original);  // City changed! Hobbies changed!
        System.out.println("Shallow copy:  " + shallow);

        // DEEP COPY
        // Reset original first
        original.getAddress().setCity("Springfield");
        original.getHobbies().remove("Gaming");

        Person deep = original.deepCopy();
        System.out.println("\nDeep copy:     " + deep);

        // Modify nested objects of deep copy
        deep.getAddress().setCity("Capital City"); // Does NOT affect original
        deep.getHobbies().add("Hiking");           // Does NOT affect original
        deep.setName("Alice (Deep)");

        System.out.println("\nAfter modifying deep copy:");
        System.out.println("Original:      " + original);  // UNCHANGED
        System.out.println("Deep copy:     " + deep);       // Changed independently
    }
}
```

**Deep Copy via Serialization (alternative approach):**
```java
import java.io.*;

// All classes must implement Serializable
public static <T extends Serializable> T deepCopyViaSerialization(T obj) {
    try {
        ByteArrayOutputStream bos = new ByteArrayOutputStream();
        ObjectOutputStream oos = new ObjectOutputStream(bos);
        oos.writeObject(obj);

        ByteArrayInputStream bis = new ByteArrayInputStream(bos.toByteArray());
        ObjectInputStream ois = new ObjectInputStream(bis);
        return (T) ois.readObject();
    } catch (IOException | ClassNotFoundException e) {
        throw new RuntimeException("Deep copy failed", e);
    }
}
```

**When to use each:**
- **Shallow copy**: When nested objects are immutable (Strings, primitives, final records)
- **Deep copy**: When you need complete independence from the original

### 🇻🇳 Tiếng Việt

**Shallow Copy (Sao chép nông):**
- Tạo object mới, copy các fields nguyên thủy (primitive) và tham chiếu (reference)
- Các reference fields **trỏ đến cùng object** với bản gốc
- Thay đổi nested object trong bản copy → ảnh hưởng đến bản gốc

**Deep Copy (Sao chép sâu):**
- Tạo object mới **hoàn toàn độc lập**
- Tất cả nested objects đều được tạo mới
- Thay đổi trong bản copy → **không ảnh hưởng** bản gốc

**Khi nào dùng:**
- Shallow copy: Khi nested objects là immutable (String, số nguyên thuỷ)
- Deep copy: Khi cần độc lập hoàn toàn, ví dụ: undo/redo history, thread safety

**Lưu ý với `Object.clone()`:** Mặc định chỉ là shallow copy. Để deep copy, phải override `clone()` và tự copy từng nested object.

---
## Q11. What are static methods and static variables? When should they be used?

### 🇬🇧 English

**Static** members belong to the **class** rather than any specific instance. They are shared across all instances and can be accessed without creating an object.

| Aspect | Static | Instance |
|--------|--------|----------|
| **Belongs to** | Class | Object instance |
| **Memory** | Allocated once (class loading) | Per instance |
| **Access** | `ClassName.member` | `objectRef.member` |
| **`this` keyword** | NOT available | Available |
| **Overriding** | Cannot be overridden (hidden) | Can be overridden |
| **Use case** | Utility methods, constants, counters | State specific to each object |

```java
// ============================================================
// Static vs Instance — Math Utilities and Counter Example
// ============================================================

public class MathHelper {
    // Static constant — shared, never changes
    public static final double PI = 3.14159265358979;
    public static final double E  = 2.71828182845904;

    // Static variable — shared counter across ALL instances
    private static int operationCount = 0;

    // Instance variable — each object has its own precision
    private int decimalPrecision;

    public MathHelper(int decimalPrecision) {
        this.decimalPrecision = decimalPrecision;
    }

    // STATIC METHOD — utility, no need for object state
    // Cannot access instance fields (no 'this')
    public static double circleArea(double radius) {
        operationCount++;  // Can access static fields
        return PI * radius * radius;
    }

    public static double power(double base, int exponent) {
        operationCount++;
        double result = 1;
        for (int i = 0; i < Math.abs(exponent); i++) {
            result *= base;
        }
        return exponent < 0 ? 1.0 / result : result;
    }

    public static boolean isPrime(int n) {
        if (n < 2) return false;
        for (int i = 2; i <= Math.sqrt(n); i++) {
            if (n % i == 0) return false;
        }
        return true;
    }

    // INSTANCE METHOD — depends on decimalPrecision (instance state)
    public String format(double value) {
        return String.format("%." + decimalPrecision + "f", value);
    }

    public String formatArea(double radius) {
        return format(circleArea(radius));  // Combines static + instance
    }

    // Static getter for shared counter
    public static int getOperationCount() { return operationCount; }
    public static void resetCounter() { operationCount = 0; }
}

// Static Factory Methods — common pattern
public class ConnectionPool {
    private static ConnectionPool instance;  // Static singleton instance
    private static final int MAX_CONNECTIONS = 10;
    private final List<String> connections;

    // Private constructor — prevent direct instantiation
    private ConnectionPool() {
        connections = new ArrayList<>();
        for (int i = 1; i <= MAX_CONNECTIONS; i++) {
            connections.add("Connection-" + i);
        }
        System.out.println("Connection pool initialized with " + MAX_CONNECTIONS + " connections");
    }

    // Static factory method — named constructor pattern
    public static ConnectionPool getInstance() {
        if (instance == null) {
            instance = new ConnectionPool();
        }
        return instance;
    }

    public String getConnection() {
        if (connections.isEmpty()) {
            throw new RuntimeException("No available connections");
        }
        return connections.remove(0);
    }

    public void releaseConnection(String conn) {
        connections.add(conn);
    }

    public static int getMaxConnections() { return MAX_CONNECTIONS; }
    public int getAvailableCount() { return connections.size(); }
}

// Static initializer block — complex initialization logic
public class DatabaseConfig {
    private static final String DB_URL;
    private static final int TIMEOUT;
    private static final Map<String, String> DEFAULTS;

    // Static initializer block — runs once when class is loaded
    static {
        DB_URL = System.getenv("DB_URL") != null
            ? System.getenv("DB_URL")
            : "jdbc:postgresql://localhost:5432/mydb";
        TIMEOUT = 30;
        DEFAULTS = new HashMap<>();
        DEFAULTS.put("pool_size", "10");
        DEFAULTS.put("charset", "UTF-8");
        DEFAULTS.put("timezone", "UTC");
        System.out.println("DatabaseConfig loaded: " + DB_URL);
    }

    public static String getDbUrl() { return DB_URL; }
    public static int getTimeout() { return TIMEOUT; }
    public static Map<String, String> getDefaults() {
        return new HashMap<>(DEFAULTS);  // Return copy for safety
    }
}

public class StaticDemo {
    public static void main(String[] args) {
        // Static methods — no object needed
        System.out.println("Circle area (r=5): " + MathHelper.circleArea(5));
        System.out.println("2^10 = " + MathHelper.power(2, 10));
        System.out.println("Is 17 prime? " + MathHelper.isPrime(17));

        // Instance method needs object
        MathHelper highPrecision = new MathHelper(4);
        MathHelper lowPrecision  = new MathHelper(1);
        System.out.println("High precision: " + highPrecision.formatArea(5)); // 78.5398
        System.out.println("Low precision:  " + lowPrecision.formatArea(5));  // 78.5

        System.out.println("Operations performed: " + MathHelper.getOperationCount()); // 5

        // Static constant
        System.out.println("PI = " + MathHelper.PI);
        System.out.println("Max connections: " + ConnectionPool.getMaxConnections());
    }
}
```

**When to use `static`:**
- ✅ Utility/helper methods (Math operations, String utils)
- ✅ Constants (`static final`)
- ✅ Factory methods
- ✅ Counters, registry, shared configuration
- ✅ Singleton instances

**When NOT to use `static`:**
- ❌ Methods that need object state
- ❌ When you need polymorphism (static methods can't be overridden)
- ❌ Mutable static fields in multithreaded code (thread-safety issues)

### 🇻🇳 Tiếng Việt

**Static member** thuộc về **class**, không phải instance. Tất cả objects của class đó chia sẻ cùng static field/method.

**Khi nào dùng `static`:**
- Phương thức tiện ích (utility): `Math.abs()`, `Collections.sort()`
- Hằng số: `static final double PI = 3.14`
- Factory methods: `ConnectionPool.getInstance()`
- Bộ đếm dùng chung: đếm số lượng object đã tạo

**Khi KHÔNG nên dùng:**
- Khi method cần truy cập trạng thái của object cụ thể
- Trong môi trường multi-thread với mutable static fields → race condition
- Khi cần đa hình (static method không thể override, chỉ có thể hide)

**Lưu ý quan trọng:** Static field là mutable global state → khó test, khó debug. Hạn chế dùng mutable static fields, chỉ dùng `static final` cho constants.

---
## Q12. What is the difference between final, finally, and finalize in Java?

### 🇬🇧 English

These three keywords sound similar but serve entirely different purposes:

| Keyword | Type | Purpose |
|---------|------|---------|
| `final` | Keyword | Restrict modification (variable, method, class) |
| `finally` | Block | Always-executed cleanup code in try-catch |
| `finalize` | Method | Called by GC before object is destroyed (deprecated) |

```java
// ============================================================
// final, finally, finalize — Examples
// ============================================================

// ---- 1. FINAL KEYWORD ----

// final CLASS — cannot be subclassed
public final class ImmutablePoint {
    private final double x;  // final field — cannot be reassigned
    private final double y;

    public ImmutablePoint(double x, double y) {
        this.x = x;
        this.y = y;
    }

    // final METHOD — cannot be overridden (but class is already final)
    public final double distanceTo(ImmutablePoint other) {
        double dx = this.x - other.x;
        double dy = this.y - other.y;
        return Math.sqrt(dx * dx + dy * dy);
    }

    public double getX() { return x; }
    public double getY() { return y; }

    @Override
    public String toString() { return "(" + x + ", " + y + ")"; }
}

// Example with final in method
public class FinalExamples {
    // final local variable
    public void demonstrateFinalVariable() {
        final int MAX_RETRIES = 3;
        // MAX_RETRIES = 4;  // Compile error! Cannot reassign final

        final List<String> names = new ArrayList<>();
        names.add("Alice");  // OK — modifying contents is allowed
        names.add("Bob");
        // names = new ArrayList<>();  // Compile error! Cannot reassign the reference
    }

    // final parameter — prevents accidental reassignment in method body
    public double calculateInterest(final double principal,
                                    final double rate,
                                    final int years) {
        // rate = 0.05;  // Compile error if uncommented
        return principal * Math.pow(1 + rate, years) - principal;
    }

    // Base class with final method
    public class Template {
        // Template method — defines algorithm, cannot be changed
        public final void executePipeline(String data) {
            String validated = validate(data);
            String processed = process(validated);
            save(processed);
        }

        protected String validate(String data) { return data.trim(); }
        protected String process(String data) { return data.toUpperCase(); }
        protected void save(String data) { System.out.println("Saving: " + data); }
    }
}

// ---- 2. FINALLY BLOCK ----
public class FinallyExamples {

    // finally always executes — even with return or exception
    public String readFile(String filename) {
        BufferedReader reader = null;
        try {
            reader = new BufferedReader(new FileReader(filename));
            String firstLine = reader.readLine();
            System.out.println("File read successfully");
            return firstLine;  // even with this return, finally STILL runs
        } catch (FileNotFoundException e) {
            System.err.println("File not found: " + filename);
            return null;
        } catch (IOException e) {
            System.err.println("IO error reading file");
            return null;
        } finally {
            // ALWAYS executes — cleanup code
            if (reader != null) {
                try {
                    reader.close();
                    System.out.println("Reader closed in finally block");
                } catch (IOException e) {
                    System.err.println("Error closing reader");
                }
            }
        }
    }

    // Modern approach: try-with-resources (preferred over finally for Closeable)
    public String readFileModern(String filename) {
        try (BufferedReader reader = new BufferedReader(new FileReader(filename))) {
            // reader is automatically closed — even if exception occurs
            return reader.readLine();
        } catch (IOException e) {
            System.err.println("Error: " + e.getMessage());
            return null;
        }
    }

    // finally with database connection
    public List<String> queryDatabase(String sql) {
        Connection conn = null;
        PreparedStatement stmt = null;
        List<String> results = new ArrayList<>();
        try {
            conn = getConnection();
            stmt = conn.prepareStatement(sql);
            ResultSet rs = stmt.executeQuery();
            while (rs.next()) {
                results.add(rs.getString(1));
            }
        } catch (SQLException e) {
            System.err.println("Query failed: " + e.getMessage());
        } finally {
            // Resource cleanup — always runs
            closeQuietly(stmt);
            closeQuietly(conn);
        }
        return results;
    }

    private void closeQuietly(AutoCloseable resource) {
        if (resource != null) {
            try { resource.close(); } catch (Exception ignored) {}
        }
    }

    private Connection getConnection() throws SQLException { return null; } // Stub
}

// ---- 3. FINALIZE METHOD (Deprecated since Java 9) ----
// Called by GC before object is collected — DO NOT rely on this
public class LegacyResource {
    private String resourceName;

    public LegacyResource(String name) {
        this.resourceName = name;
        System.out.println("Resource opened: " + name);
    }

    // DEPRECATED — unpredictable, may never be called
    // Never guarantee resource cleanup with finalize()
    @Override
    @Deprecated
    protected void finalize() throws Throwable {
        try {
            System.out.println("finalize() called for: " + resourceName);
            // Release native resources here if absolutely necessary
        } finally {
            super.finalize();
        }
    }
}

// Modern replacement: AutoCloseable
public class ModernResource implements AutoCloseable {
    private final String resourceName;
    private boolean closed = false;

    public ModernResource(String name) {
        this.resourceName = name;
        System.out.println("Resource opened: " + name);
    }

    public void doWork() {
        if (closed) throw new IllegalStateException("Resource is closed");
        System.out.println("Working with: " + resourceName);
    }

    @Override
    public void close() {
        if (!closed) {
            closed = true;
            System.out.println("Resource closed: " + resourceName);
        }
    }
}

// Usage
public class CleanupDemo {
    public static void main(String[] args) {
        // Modern resource management — preferred
        try (ModernResource res = new ModernResource("FileHandle")) {
            res.doWork();
        } // close() called automatically here
    }
}
```

**Summary:**
- `final`: Immutability and restriction — prevent reassignment, inheritance, or overriding
- `finally`: Guaranteed cleanup — runs after try/catch regardless of exceptions
- `finalize()`: **Deprecated** — don't use; use `AutoCloseable` and try-with-resources instead

### 🇻🇳 Tiếng Việt

**`final` (từ khóa):**
- **Biến `final`**: Không thể gán lại sau khi khởi tạo
- **Phương thức `final`**: Không thể override ở lớp con
- **Lớp `final`**: Không thể kế thừa (ví dụ: `String`, `Integer`)

**`finally` (khối lệnh):**
- Luôn được thực thi sau `try/catch`, dù có exception hay không, dù có `return` hay không
- Dùng để dọn dẹp tài nguyên: đóng file, database connection
- **Cách hiện đại hơn**: Dùng `try-with-resources` với `AutoCloseable`

**`finalize()` (phương thức — đã lỗi thời):**
- Được JVM gọi trước khi GC thu hồi object
- **Không nên dùng**: Không đảm bảo khi nào được gọi, ảnh hưởng hiệu năng
- **Thay thế bằng**: Implement `AutoCloseable` và dùng `try-with-resources`

---
## Q13. What is an enum in Java, and when should it be used?

### 🇬🇧 English

An **enum** (enumeration) is a special type that represents a fixed set of named constants. Enums in Java are type-safe, can have fields, methods, and constructors, making them far more powerful than simple integer constants.

```java
// ============================================================
// Enums — Comprehensive Examples
// ============================================================

// BASIC ENUM — Days of the week
public enum DayOfWeek {
    MONDAY, TUESDAY, WEDNESDAY, THURSDAY, FRIDAY, SATURDAY, SUNDAY;

    public boolean isWeekend() {
        return this == SATURDAY || this == SUNDAY;
    }

    public boolean isWeekday() {
        return !isWeekend();
    }
}

// ENUM WITH FIELDS AND METHODS — Planet example
public enum Planet {
    MERCURY(3.303e+23, 2.4397e6),
    VENUS  (4.869e+24, 6.0518e6),
    EARTH  (5.976e+24, 6.37814e6),
    MARS   (6.421e+23, 3.3972e6),
    JUPITER(1.9e+27,   7.1492e7),
    SATURN (5.688e+26, 6.0268e7),
    URANUS (8.686e+25, 2.5559e7),
    NEPTUNE(1.024e+26, 2.4746e7);

    private final double mass;    // kg
    private final double radius;  // meters
    static final double G = 6.67300E-11;

    // Enum constructor — always private
    Planet(double mass, double radius) {
        this.mass = mass;
        this.radius = radius;
    }

    double surfaceGravity() {
        return G * mass / (radius * radius);
    }

    double surfaceWeight(double otherMass) {
        return otherMass * surfaceGravity();
    }

    public double getMass() { return mass; }
    public double getRadius() { return radius; }
}

// ENUM WITH ABSTRACT METHOD — Strategy per enum value
public enum Operation {
    ADD("+") {
        @Override
        public double apply(double x, double y) { return x + y; }
    },
    SUBTRACT("-") {
        @Override
        public double apply(double x, double y) { return x - y; }
    },
    MULTIPLY("*") {
        @Override
        public double apply(double x, double y) { return x * y; }
    },
    DIVIDE("/") {
        @Override
        public double apply(double x, double y) {
            if (y == 0) throw new ArithmeticException("Division by zero");
            return x / y;
        }
    };

    private final String symbol;

    Operation(String symbol) { this.symbol = symbol; }

    public String getSymbol() { return symbol; }

    // Each constant MUST implement this
    public abstract double apply(double x, double y);

    @Override
    public String toString() {
        return String.format("%.2f %s %.2f = %.2f",
            0.0, symbol, 0.0, 0.0); // placeholder
    }
}

// ENUM IN SWITCH — Clean finite state machine
public enum TrafficLight {
    RED(30),
    YELLOW(5),
    GREEN(25);

    private final int durationSeconds;

    TrafficLight(int duration) { this.durationSeconds = duration; }

    public int getDurationSeconds() { return durationSeconds; }

    public TrafficLight next() {
        return switch (this) {
            case RED    -> GREEN;
            case GREEN  -> YELLOW;
            case YELLOW -> RED;
        };
    }

    public String getInstruction() {
        return switch (this) {
            case RED    -> "STOP";
            case YELLOW -> "CAUTION";
            case GREEN  -> "GO";
        };
    }
}

// ENUM AS SINGLETON (Thread-safe, serialization-safe)
public enum AppConfig {
    INSTANCE;  // Single instance

    private String dbUrl = "jdbc:postgresql://localhost/prod";
    private int maxRetries = 3;
    private boolean debugMode = false;

    public String getDbUrl() { return dbUrl; }
    public void setDbUrl(String url) { this.dbUrl = url; }
    public int getMaxRetries() { return maxRetries; }
    public boolean isDebugMode() { return debugMode; }
    public void setDebugMode(boolean debug) { this.debugMode = debug; }
}

public class EnumDemo {
    public static void main(String[] args) {
        // Basic usage
        DayOfWeek today = DayOfWeek.WEDNESDAY;
        System.out.println(today + " is weekend: " + today.isWeekend()); // false

        // Iterate enum values
        System.out.println("\nWeekend days:");
        for (DayOfWeek day : DayOfWeek.values()) {
            if (day.isWeekend()) System.out.println("  " + day);
        }

        // Enum with fields
        double earthWeight = 75.0;
        double mass = earthWeight / Planet.EARTH.surfaceGravity();
        System.out.println("\nWeight on each planet (for " + earthWeight + "kg on Earth):");
        for (Planet p : Planet.values()) {
            System.out.printf("  %-8s: %6.2f N%n", p, p.surfaceWeight(mass));
        }

        // Enum with abstract method (Strategy pattern)
        double x = 10, y = 3;
        for (Operation op : Operation.values()) {
            System.out.printf("%.1f %s %.1f = %.2f%n",
                x, op.getSymbol(), y, op.apply(x, y));
        }

        // Traffic light state machine
        TrafficLight light = TrafficLight.RED;
        System.out.println("\nTraffic light simulation:");
        for (int i = 0; i < 6; i++) {
            System.out.printf("  %s (%ds) — %s%n",
                light, light.getDurationSeconds(), light.getInstruction());
            light = light.next();
        }

        // Enum singleton
        AppConfig.INSTANCE.setDebugMode(true);
        System.out.println("Debug mode: " + AppConfig.INSTANCE.isDebugMode());

        // Enum by name (throws IllegalArgumentException if not found)
        DayOfWeek friday = DayOfWeek.valueOf("FRIDAY");
        System.out.println("Parsed: " + friday);

        // Enum ordinal (use carefully — fragile if order changes)
        System.out.println("MONDAY ordinal: " + DayOfWeek.MONDAY.ordinal()); // 0
    }
}
```

**When to use Enums:**
- ✅ Fixed, known set of constants (days, months, status codes, colors)
- ✅ Replace magic numbers/strings
- ✅ Type-safe alternatives to integer flags
- ✅ State machines and strategy patterns per constant
- ✅ Thread-safe singleton (enum singleton)

**Avoid enums when:**
- ❌ The set of values changes at runtime
- ❌ You need to load values from a database

### 🇻🇳 Tiếng Việt

**Enum** là kiểu đặc biệt đại diện cho tập hợp hằng số cố định, có tên. Khác với các ngôn ngữ khác, enum trong Java rất mạnh mẽ — có thể có fields, methods và constructors.

**Khi nào dùng Enum:**
- Trạng thái cố định: `OrderStatus.PENDING`, `TrafficLight.RED`
- Thay thế magic numbers: `if (status == 1)` → `if (status == OrderStatus.PENDING)`
- Finite State Machine: mỗi enum value định nghĩa `next()` method
- Singleton thread-safe: Enum singleton là cách implement Singleton tốt nhất

**Ưu điểm so với hằng số `int/String`:**
- Type-safe: không thể truyền nhầm giá trị
- Có thể có behavior (methods)
- Switch expression hỗ trợ tốt với enum
- Serialization an toàn

**Lưu ý:** Tránh dùng `ordinal()` cho logic nghiệp vụ — nếu thứ tự enum thay đổi, code sẽ bị lỗi. Dùng field riêng thay thế.

---
## Q14. How does Java handle memory management and garbage collection?

### 🇬🇧 English

Java uses **automatic memory management** via the **Garbage Collector (GC)**. The JVM manages the heap and reclaims memory from objects that are no longer reachable.

#### JVM Memory Structure:
- **Heap**: Where objects live. Divided into Young Generation (Eden + Survivor) and Old Generation
- **Stack**: Method call frames, local variables, references (per thread)
- **Method Area/Metaspace**: Class metadata, static variables
- **Program Counter**: Current instruction per thread
- **Native Method Stack**: For native (C/C++) code

```java
// ============================================================
// Memory Management and GC Concepts in Java
// ============================================================

public class MemoryManagementDemo {

    // Objects created in methods are eligible for GC when the method returns
    // (if no other references exist)
    public static void demonstrateGCEligibility() {
        // This object is created on the heap
        StringBuilder sb = new StringBuilder("Hello");
        sb.append(" World");
        System.out.println(sb.toString());
        // When this method returns, 'sb' goes out of scope
        // The StringBuilder object becomes eligible for GC
    }

    // STRONG REFERENCES — default, prevents GC
    public static void strongReference() {
        Object obj = new Object();  // Strong reference
        // obj is NOT eligible for GC as long as 'obj' variable is in scope
        obj = null;  // Now eligible for GC (if no other references)
    }

    // WEAK REFERENCES — collected at next GC cycle
    public static void weakReferenceExample() {
        String data = new String("Important Data");

        // WeakReference — GC can collect the referent anytime
        java.lang.ref.WeakReference<String> weakRef =
            new java.lang.ref.WeakReference<>(data);

        data = null;  // Remove strong reference

        // May return null if GC has run
        String retrieved = weakRef.get();
        System.out.println("Retrieved: " + retrieved);  // May be null

        System.gc();  // Suggest GC (not guaranteed to run immediately)
        System.out.println("After GC: " + weakRef.get());  // Likely null
    }

    // SOFT REFERENCES — collected only when memory is low
    public static void softReferenceExample() {
        byte[] largeData = new byte[1024 * 1024]; // 1MB
        java.lang.ref.SoftReference<byte[]> softRef =
            new java.lang.ref.SoftReference<>(largeData);

        largeData = null;  // Remove strong reference

        // SoftReference is kept in memory as long as there's enough heap
        // Useful for memory-sensitive caches
        byte[] cached = softRef.get();
        if (cached != null) {
            System.out.println("Cache hit: " + cached.length + " bytes");
        } else {
            System.out.println("Cache miss — data was GC'd");
        }
    }

    // MEMORY LEAK EXAMPLE — static collections holding references
    // Anti-pattern: unbounded static cache
    private static final Map<String, Object> STATIC_CACHE = new HashMap<>();

    public static void potentialMemoryLeak(String key, Object value) {
        STATIC_CACHE.put(key, value);
        // Objects in STATIC_CACHE are NEVER GC'd (as long as class is loaded)
        // Fix: Use WeakHashMap, or implement eviction policy
    }

    // FIX: Use WeakHashMap — keys are weakly referenced
    private static final Map<String, Object> SAFE_CACHE =
        new java.util.WeakHashMap<>();
}

// Object lifecycle example
public class ObjectLifecycle {
    private static int count = 0;
    private final int id;

    public ObjectLifecycle() {
        id = ++count;
        System.out.println("Object #" + id + " created");
    }

    public void process() {
        System.out.println("Object #" + id + " processing...");
    }

    // Modern cleanup: implement AutoCloseable instead of finalize
    // (not shown here for brevity)
}

// Practical: Avoiding common memory pitfalls
public class MemoryBestPractices {

    // 1. CLOSE RESOURCES — use try-with-resources
    public void readFileCorrectly(String path) throws IOException {
        try (InputStream is = new FileInputStream(path);
             BufferedReader reader = new BufferedReader(new InputStreamReader(is))) {
            String line;
            while ((line = reader.readLine()) != null) {
                process(line);
            }
        } // Both reader and is are automatically closed
    }

    // 2. AVOID HOLDING LARGE OBJECTS LONGER THAN NEEDED
    public void processLargeDataset() {
        List<String> largeList = loadMillionRecords();
        try {
            processRecords(largeList);
        } finally {
            largeList = null;  // Help GC by removing reference early
            // Note: JIT compiler might optimize this away, but it signals intent
        }
    }

    // 3. REUSE OBJECTS — StringBuilder instead of String concatenation
    public String buildReportBad(List<String> items) {
        String result = "";  // BAD: creates new String object each iteration
        for (String item : items) {
            result += item + "\n";  // O(n²) memory allocation
        }
        return result;
    }

    public String buildReportGood(List<String> items) {
        StringBuilder sb = new StringBuilder(items.size() * 20);  // Pre-sized
        for (String item : items) {
            sb.append(item).append('\n');  // O(n) — single StringBuilder
        }
        return sb.toString();
    }

    // 4. OBJECT POOLING for expensive objects
    // Example: database connections, thread pools (use existing libraries)

    private void process(String line) {}
    private List<String> loadMillionRecords() { return new ArrayList<>(); }
    private void processRecords(List<String> records) {}
}
```

#### Garbage Collection Algorithms:
| Algorithm | Generation | Description |
|-----------|-----------|-------------|
| **Serial GC** | All | Single-threaded, simple |
| **Parallel GC** | All | Multi-threaded, throughput-focused |
| **G1 GC** | All | Low-pause, predictable (default since Java 9) |
| **ZGC** | All | Ultra-low latency (<10ms pauses, Java 15+) |
| **Shenandoah** | All | Concurrent, low-pause (OpenJDK) |

**JVM Tuning Flags:**
```bash
-Xms512m          # Initial heap size
-Xmx2g            # Maximum heap size
-XX:+UseG1GC      # Use G1 Garbage Collector
-XX:MaxGCPauseMillis=200  # Target max GC pause
-XX:+PrintGCDetails       # Log GC events
```

### 🇻🇳 Tiếng Việt

Java quản lý bộ nhớ tự động thông qua **Garbage Collector (GC)**. Lập trình viên không cần giải phóng bộ nhớ thủ công như C/C++.

**Cấu trúc bộ nhớ JVM:**
- **Heap**: Nơi lưu trữ objects. Gồm Young Generation (Eden + Survivor) và Old Generation
- **Stack**: Lưu method call frames, biến local (mỗi thread có stack riêng)
- **Metaspace**: Metadata của classes, static variables

**Khi nào object bị GC thu hồi?**
Khi không còn **bất kỳ strong reference** nào trỏ đến object — tức là không còn "đường dẫn" nào từ GC Root đến object đó.

**GC Root bao gồm:** Stack variables, static fields, JNI references.

**Các loại reference:**
- `Strong` (mặc định): GC không bao giờ thu hồi
- `SoftReference`: Giữ đến khi sắp hết heap — dùng cho cache
- `WeakReference`: Thu hồi tại GC cycle tiếp theo — dùng cho canonical maps
- `PhantomReference`: Sau khi finalized — dùng cho cleanup nâng cao

**Tránh memory leak:** Đừng giữ references không cần thiết trong static collections, selectors, listeners. Luôn unregister listeners khi không dùng.

---
## Q15. What is the equals() method in Java, and how is it different from ==?

### 🇬🇧 English

| Aspect | `==` operator | `equals()` method |
|--------|--------------|------------------|
| **Compares** | References (memory address) | Object content/value |
| **For primitives** | Value comparison | N/A (primitives) |
| **For objects** | Same object in memory? | Logical equality |
| **Overrideable** | No | Yes |
| **Default behavior** | Reference equality | Same as `==` (Object class) |

```java
// ============================================================
// equals() vs == and proper implementation
// ============================================================

// Proper equals() implementation with all edge cases
public class Product {
    private final String sku;
    private final String name;
    private final double price;
    private final String category;

    public Product(String sku, String name, double price, String category) {
        this.sku = sku;
        this.name = name;
        this.price = price;
        this.category = category;
    }

    // CORRECT equals() implementation — follows the contract:
    // 1. Reflexive:  x.equals(x) must be true
    // 2. Symmetric:  x.equals(y) iff y.equals(x)
    // 3. Transitive: if x.equals(y) and y.equals(z), then x.equals(z)
    // 4. Consistent: multiple calls return same result
    // 5. Null-safe:  x.equals(null) must return false (never throw NPE)
    @Override
    public boolean equals(Object obj) {
        // 1. Self-check optimization
        if (this == obj) return true;

        // 2. Null check
        if (obj == null) return false;

        // 3. Type check — use instanceof (handles subclasses)
        if (!(obj instanceof Product)) return false;

        // 4. Cast and compare significant fields
        Product other = (Product) obj;
        return Objects.equals(this.sku, other.sku)  // SKU uniquely identifies a product
            && Objects.equals(this.name, other.name)
            && Double.compare(this.price, other.price) == 0  // Use Double.compare for doubles
            && Objects.equals(this.category, other.category);
    }

    // ALWAYS override hashCode when you override equals!
    @Override
    public int hashCode() {
        // Objects.hash() creates a consistent hash from multiple fields
        return Objects.hash(sku, name, price, category);
    }

    // Modern approach using Java 16+ records (auto-generates equals/hashCode)
    // public record Product(String sku, String name, double price, String category) {}

    @Override
    public String toString() {
        return String.format("Product{sku='%s', name='%s', price=%.2f}", sku, name, price);
    }

    public String getSku() { return sku; }
    public String getName() { return name; }
    public double getPrice() { return price; }
}

public class EqualsDemo {
    public static void main(String[] args) {
        // ---- String comparison ----
        String s1 = "Hello";
        String s2 = "Hello";               // Same string pool object
        String s3 = new String("Hello");   // Different object, same content

        System.out.println("s1 == s2: " + (s1 == s2));         // true (pool)
        System.out.println("s1 == s3: " + (s1 == s3));         // false (different ref)
        System.out.println("s1.equals(s2): " + s1.equals(s2)); // true
        System.out.println("s1.equals(s3): " + s1.equals(s3)); // true

        // ---- Custom object comparison ----
        Product p1 = new Product("SKU-001", "Laptop", 999.99, "Electronics");
        Product p2 = new Product("SKU-001", "Laptop", 999.99, "Electronics");
        Product p3 = p1;  // Same reference

        System.out.println("\np1 == p2: " + (p1 == p2));         // false (different objects)
        System.out.println("p1 == p3: " + (p1 == p3));            // true (same reference)
        System.out.println("p1.equals(p2): " + p1.equals(p2));    // true (same content)
        System.out.println("p1.equals(null): " + p1.equals(null)); // false (null-safe)

        // ---- HashSet requires consistent equals + hashCode ----
        Set<Product> productSet = new HashSet<>();
        productSet.add(p1);
        productSet.add(p2);  // Should not be added (duplicate per equals)
        System.out.println("\nSet size (should be 1): " + productSet.size()); // 1

        // ---- HashMap lookup ----
        Map<Product, Integer> inventory = new HashMap<>();
        inventory.put(p1, 50);
        System.out.println("Inventory for p2: " + inventory.get(p2)); // 50 (works because equals+hashCode)

        // ---- Primitive == compares values ----
        int a = 5, b = 5;
        System.out.println("\n5 == 5: " + (a == b));  // true (value comparison)

        // ---- Integer cache trap ----
        Integer i1 = 127;
        Integer i2 = 127;
        Integer i3 = 128;
        Integer i4 = 128;
        System.out.println("127 == 127: " + (i1 == i2));     // true (cached)
        System.out.println("128 == 128: " + (i3 == i4));     // false (not cached!)
        System.out.println("128.equals(128): " + i3.equals(i4)); // true (always use equals!)
    }
}
```

**The equals/hashCode Contract:**
> If `a.equals(b)` is `true`, then `a.hashCode()` **must** equal `b.hashCode()`
> The reverse is NOT required (hash collisions are allowed)

Breaking this contract causes subtle bugs in `HashMap`, `HashSet`, and `Hashtable`.

### 🇻🇳 Tiếng Việt

**`==` toán tử:** So sánh **tham chiếu** (địa chỉ bộ nhớ). Hai biến == nhau khi cùng trỏ đến một object trong heap.

**`equals()` phương thức:** So sánh **nội dung logic**. Mặc định trong `Object` cũng là so sánh tham chiếu, nhưng có thể override.

**Bẫy Integer caching:** Java cache `Integer` từ -128 đến 127. `Integer i1 = 127; Integer i2 = 127; i1 == i2` là `true`, nhưng `Integer i3 = 128; Integer i4 = 128; i3 == i4` là `false`. Luôn dùng `equals()` cho objects!

**Hợp đồng `equals()`:**
1. Reflexive: `x.equals(x)` = true
2. Symmetric: `x.equals(y)` ↔ `y.equals(x)`
3. Transitive: `x.equals(y)` và `y.equals(z)` → `x.equals(z)`
4. Null-safe: `x.equals(null)` = false

**Quy tắc vàng:** Khi override `equals()`, **bắt buộc** phải override `hashCode()` theo cùng logic. Nếu không, `HashSet`/`HashMap` sẽ hoạt động sai.

---
## Q16. What are Java Beans and POJOs? How are they used?

### 🇬🇧 English

| Concept | Definition |
|---------|-----------|
| **POJO** | Plain Old Java Object — any regular Java class, no restrictions |
| **Java Bean** | A POJO following specific conventions for frameworks (Spring, Hibernate, etc.) |

**Java Bean Conventions:**
1. Default (no-argument) constructor
2. Private fields
3. Public getters/setters following naming convention (`getXxx()`, `setXxx()`, `isXxx()` for boolean)
4. Implements `Serializable` (optional but recommended)

```java
// ============================================================
// POJO vs Java Bean
// ============================================================

// POJO: Simple class, no conventions required
class SimplePojo {
    public String name;   // public field — valid POJO
    public int age;

    // Any constructor is fine
    public SimplePojo(String name, int age) {
        this.name = name;
        this.age = age;
    }
    // No getters/setters required
}

// JAVA BEAN: Follows strict conventions for framework compatibility
import java.io.Serializable;

public class UserBean implements Serializable {
    private static final long serialVersionUID = 1L;  // For Serializable

    // Private fields (encapsulation)
    private Long id;
    private String firstName;
    private String lastName;
    private String email;
    private boolean active;
    private java.time.LocalDate birthDate;

    // 1. REQUIRED: No-arg constructor (must be public)
    public UserBean() {
        // Default values if needed
        this.active = true;
    }

    // Additional constructors allowed
    public UserBean(String firstName, String lastName, String email) {
        this();  // Call no-arg constructor
        this.firstName = firstName;
        this.lastName = lastName;
        this.email = email;
    }

    // 2. GETTERS — naming: getFieldName() for regular fields
    public Long getId() { return id; }
    public String getFirstName() { return firstName; }
    public String getLastName() { return lastName; }
    public String getEmail() { return email; }
    public java.time.LocalDate getBirthDate() { return birthDate; }

    // 3. For boolean fields: isFieldName() — NOT getActive()
    public boolean isActive() { return active; }

    // 4. SETTERS — void, one parameter
    public void setId(Long id) { this.id = id; }
    public void setFirstName(String firstName) { this.firstName = firstName; }
    public void setLastName(String lastName) { this.lastName = lastName; }
    public void setEmail(String email) { this.email = email; }
    public void setActive(boolean active) { this.active = active; }
    public void setBirthDate(java.time.LocalDate birthDate) { this.birthDate = birthDate; }

    // Derived property — no field, but follows getter convention
    public String getFullName() {
        return firstName + " " + lastName;
    }

    @Override
    public String toString() {
        return String.format("UserBean{id=%d, name='%s', email='%s', active=%b}",
            id, getFullName(), email, active);
    }

    @Override
    public boolean equals(Object o) {
        if (this == o) return true;
        if (!(o instanceof UserBean)) return false;
        UserBean user = (UserBean) o;
        return Objects.equals(id, user.id);  // Equality based on ID
    }

    @Override
    public int hashCode() {
        return Objects.hash(id);
    }
}

// MODERN ALTERNATIVE: Java Records (Java 16+)
// Immutable, auto-generates constructor, getters, equals, hashCode, toString
public record ProductRecord(String sku, String name, double price, String category) {
    // Compact constructor for validation
    public ProductRecord {
        if (sku == null || sku.isBlank()) throw new IllegalArgumentException("SKU required");
        if (price < 0) throw new IllegalArgumentException("Price cannot be negative");
        name = name.trim();  // Normalize in compact constructor
    }

    // Additional methods allowed
    public double priceWithTax(double taxRate) {
        return price * (1 + taxRate);
    }
}

// DTO (Data Transfer Object) — a specific use of Java Bean
// Used to transfer data between layers (Controller → Service → Repository)
public class UserDTO {
    private Long id;
    private String username;
    private String email;
    // No password field — security: don't expose sensitive data in DTO

    public UserDTO() {}

    public UserDTO(Long id, String username, String email) {
        this.id = id;
        this.username = username;
        this.email = email;
    }

    public Long getId() { return id; }
    public String getUsername() { return username; }
    public String getEmail() { return email; }
    public void setId(Long id) { this.id = id; }
    public void setUsername(String username) { this.username = username; }
    public void setEmail(String email) { this.email = email; }
}

public class BeanDemo {
    public static void main(String[] args) {
        // Java Bean usage
        UserBean user = new UserBean();  // No-arg constructor
        user.setId(1L);
        user.setFirstName("Alice");
        user.setLastName("Johnson");
        user.setEmail("alice@example.com");
        System.out.println(user);
        System.out.println("Full name: " + user.getFullName());

        // Java Record (modern alternative)
        ProductRecord product = new ProductRecord("SKU-001", "  Laptop  ", 999.99, "Electronics");
        System.out.println(product);
        System.out.println("Price with 10% tax: " + product.priceWithTax(0.10));

        // Records are immutable
        // product = product with new sku("SKU-002");  // Use record copy syntax (Java 16+)
        ProductRecord updated = new ProductRecord("SKU-002", product.name(),
            product.price(), product.category());
    }
}
```

**Frameworks that depend on Java Bean conventions:**
- **Spring Framework**: Dependency injection, MVC model binding, JPA entities
- **Hibernate/JPA**: ORM entity mapping
- **Jackson/Gson**: JSON serialization/deserialization
- **JSP/Thymeleaf**: Template engines use getter/setter conventions

### 🇻🇳 Tiếng Việt

**POJO (Plain Old Java Object):** Class Java thông thường, không kế thừa framework-specific class, không tuân theo quy tắc đặc biệt.

**Java Bean:** POJO tuân theo các quy tắc:
1. Constructor không tham số (no-arg constructor)
2. Fields private
3. Getters/Setters public theo naming convention
4. Implement `Serializable` (tùy chọn)

**Tại sao quan trọng:**
- Spring tự động inject dependencies dựa trên setters/getters
- Jackson tự động serialize/deserialize JSON nhờ getters/setters
- JPA/Hibernate map database columns vào fields thông qua setters

**Xu hướng hiện đại:** Java 16+ giới thiệu **Records** — cú pháp ngắn gọn tạo immutable objects với constructor, getters, equals, hashCode, toString được tự động tạo. Thích hợp cho DTOs và Value Objects.

---
## Q17. What is the role of the toString() method in Java?

### 🇬🇧 English

`toString()` is defined in `java.lang.Object` and is called when an object needs to be represented as a `String` — in print statements, string concatenation, logging, and debugging.

```java
// ============================================================
// toString() — Best Practices and Examples
// ============================================================

public class Order {
    private final String orderId;
    private final String customerId;
    private final List<OrderItem> items;
    private OrderStatus status;
    private java.time.LocalDateTime createdAt;

    public Order(String orderId, String customerId) {
        this.orderId = orderId;
        this.customerId = customerId;
        this.items = new ArrayList<>();
        this.status = OrderStatus.PENDING;
        this.createdAt = java.time.LocalDateTime.now();
    }

    public void addItem(String productName, int quantity, double price) {
        items.add(new OrderItem(productName, quantity, price));
    }

    public double getTotal() {
        return items.stream().mapToDouble(OrderItem::getSubtotal).sum();
    }

    // GOOD toString() — includes all meaningful fields
    // Clear format, useful for debugging
    @Override
    public String toString() {
        return String.format(
            "Order{id='%s', customerId='%s', status=%s, items=%d, total=$%.2f, created=%s}",
            orderId, customerId, status, items.size(),
            getTotal(), createdAt.toLocalDate()
        );
    }

    // Inner classes
    public static class OrderItem {
        private final String productName;
        private final int quantity;
        private final double unitPrice;

        public OrderItem(String productName, int quantity, double unitPrice) {
            this.productName = productName;
            this.quantity = quantity;
            this.unitPrice = unitPrice;
        }

        public double getSubtotal() { return quantity * unitPrice; }

        @Override
        public String toString() {
            return String.format("%s x%d @ $%.2f = $%.2f",
                productName, quantity, unitPrice, getSubtotal());
        }
    }

    public enum OrderStatus { PENDING, CONFIRMED, SHIPPED, DELIVERED, CANCELLED }
}

// Using toString() in various contexts
public class ToStringDemo {
    public static void main(String[] args) {
        Order order = new Order("ORD-2024-001", "CUST-123");
        order.addItem("Laptop", 1, 999.99);
        order.addItem("Mouse", 2, 29.99);

        // Implicit toString() calls
        System.out.println(order);          // prints order.toString()
        System.out.println("Order: " + order); // string concatenation triggers toString()

        // In logging
        // logger.info("Processing order: {}", order); // SLF4J uses toString()

        // Without toString() — useless default output
        // Order@6d06d69c — memory address, not helpful

        // String.valueOf() uses toString() safely (handles null)
        Order nullOrder = null;
        System.out.println(String.valueOf(nullOrder)); // "null" — no NPE
        // System.out.println(nullOrder.toString());   // NullPointerException!

        // Objects.toString() with default value
        System.out.println(java.util.Objects.toString(nullOrder, "NO ORDER")); // "NO ORDER"
    }
}

// StringBuilder-based toString for performance in complex objects
public class LargeObject {
    private String field1, field2, field3;
    private List<String> items;
    private Map<String, Integer> counters;

    @Override
    public String toString() {
        // Use StringBuilder for efficiency when building complex strings
        StringBuilder sb = new StringBuilder("LargeObject{");
        sb.append("field1='").append(field1).append("', ");
        sb.append("field2='").append(field2).append("', ");
        sb.append("field3='").append(field3).append("', ");
        sb.append("items=").append(items).append(", ");
        sb.append("counters=").append(counters);
        sb.append('}');
        return sb.toString();
    }
}
```

**Best Practices for toString():**
- ✅ Include all significant fields that identify the object
- ✅ Use `String.format()` for readability
- ✅ Avoid calling methods that could throw exceptions or have side effects
- ✅ Use `Objects.toString(field, "N/A")` for nullable fields
- ❌ Don't include sensitive data (passwords, credit card numbers)
- ❌ Don't include all fields if the class is large — include identifying ones

### 🇻🇳 Tiếng Việt

`toString()` được định nghĩa trong `Object` và được gọi tự động khi:
- Dùng trong `System.out.println(obj)`
- Nối chuỗi: `"Object: " + obj`
- Logging frameworks
- Debugging trong IDE

**Nếu không override:** Java in ra `ClassName@hashcode` (ví dụ: `Order@6d06d69c`) — không có ý nghĩa.

**Nguyên tắc khi implement:**
- Bao gồm các fields quan trọng xác định object
- Dùng `String.format()` cho dễ đọc
- KHÔNG bao gồm dữ liệu nhạy cảm (mật khẩu, số thẻ)
- Dùng `Objects.toString(field, "N/A")` cho nullable fields

---
## Q18. What is a singleton class, and how can it be implemented?

### 🇬🇧 English

A **Singleton** ensures that a class has only **one instance** throughout the application, and provides a global access point to it.

**Common Use Cases:** Configuration manager, logging service, connection pool, cache, registry.

```java
// ============================================================
// Singleton — Multiple Implementation Approaches
// ============================================================

// APPROACH 1: Eager Initialization (Thread-safe, simple)
// Instance created at class loading time
public class EagerSingleton {
    // Created immediately when class is loaded
    private static final EagerSingleton INSTANCE = new EagerSingleton();

    private EagerSingleton() {
        System.out.println("EagerSingleton created");
    }

    public static EagerSingleton getInstance() {
        return INSTANCE;
    }

    public void doWork() {
        System.out.println("EagerSingleton working...");
    }
}

// APPROACH 2: Lazy Initialization (NOT thread-safe — single-threaded only)
public class LazySingleton {
    private static LazySingleton instance;  // null initially

    private LazySingleton() {}

    public static LazySingleton getInstance() {
        if (instance == null) {
            instance = new LazySingleton();  // Created on first call
        }
        return instance;
        // BUG: Two threads can both see instance==null and create two instances!
    }
}

// APPROACH 3: Thread-safe — Synchronized Method (safe but slow)
public class SynchronizedSingleton {
    private static SynchronizedSingleton instance;

    private SynchronizedSingleton() {}

    // synchronized ensures only one thread enters at a time
    // But this adds overhead on EVERY call — unnecessary after first init
    public static synchronized SynchronizedSingleton getInstance() {
        if (instance == null) {
            instance = new SynchronizedSingleton();
        }
        return instance;
    }
}

// APPROACH 4: Double-Checked Locking (DCL) — Preferred for lazy + thread-safe
public class DCLSingleton {
    // volatile: ensures visibility across threads (prevents instruction reordering)
    private static volatile DCLSingleton instance;

    private DCLSingleton() {
        // Protection against reflection attacks
        if (instance != null) {
            throw new IllegalStateException("Use getInstance()");
        }
    }

    public static DCLSingleton getInstance() {
        if (instance == null) {                   // First check (no lock)
            synchronized (DCLSingleton.class) {   // Lock only when null
                if (instance == null) {            // Second check (under lock)
                    instance = new DCLSingleton();
                }
            }
        }
        return instance;
    }
}

// APPROACH 5: Bill Pugh / Initialization-on-demand holder (Elegant + Thread-safe)
// Uses JVM class loading guarantee — best practice for most cases
public class BillPughSingleton {
    private BillPughSingleton() {}

    // Inner class is not loaded until getInstance() is called
    private static class SingletonHolder {
        private static final BillPughSingleton INSTANCE = new BillPughSingleton();
    }

    public static BillPughSingleton getInstance() {
        return SingletonHolder.INSTANCE;  // JVM guarantees thread-safe initialization
    }

    public String getVersion() { return "1.0.0"; }
}

// APPROACH 6: ENUM SINGLETON — Best for preventing reflection/serialization attacks
// Recommended by Joshua Bloch in "Effective Java"
public enum EnumSingleton {
    INSTANCE;  // The singleton

    private String configValue = "default";
    private final Map<String, String> settings = new HashMap<>();

    // Cannot use constructor with initialization logic in enum easily
    // But can use instance initializer block
    {
        settings.put("timeout", "30");
        settings.put("maxRetries", "3");
    }

    // Enum singleton methods
    public String getConfigValue() { return configValue; }
    public void setConfigValue(String value) { configValue = value; }
    public String getSetting(String key) { return settings.get(key); }

    // Enum is automatically:
    // - Thread-safe (guaranteed by JVM)
    // - Serialization-safe (JVM handles serialization correctly)
    // - Reflection-safe (cannot call private constructor via reflection on enum)
}

// PRACTICAL EXAMPLE: Application Configuration Singleton
public class AppConfiguration {
    private static volatile AppConfiguration instance;

    // Configuration properties
    private final String appName;
    private final String version;
    private final String environment;
    private final Map<String, String> properties;

    private AppConfiguration() {
        // Load from properties file / environment variables
        this.appName = System.getProperty("app.name", "MyApp");
        this.version = System.getProperty("app.version", "1.0.0");
        this.environment = System.getProperty("app.env", "development");
        this.properties = new HashMap<>();
        loadProperties();
        System.out.println("Configuration loaded for: " + appName + " v" + version);
    }

    private void loadProperties() {
        // Simulated configuration loading
        properties.put("db.url", "jdbc:postgresql://localhost/mydb");
        properties.put("db.pool.size", "10");
        properties.put("cache.ttl", "3600");
    }

    public static AppConfiguration getInstance() {
        if (instance == null) {
            synchronized (AppConfiguration.class) {
                if (instance == null) {
                    instance = new AppConfiguration();
                }
            }
        }
        return instance;
    }

    public String getAppName() { return appName; }
    public String getVersion() { return version; }
    public String getEnvironment() { return environment; }
    public String getProperty(String key) { return properties.get(key); }
    public String getProperty(String key, String defaultValue) {
        return properties.getOrDefault(key, defaultValue);
    }

    public boolean isDevelopment() { return "development".equals(environment); }
    public boolean isProduction() { return "production".equals(environment); }
}

public class SingletonDemo {
    public static void main(String[] args) {
        // Multiple calls return the same instance
        AppConfiguration config1 = AppConfiguration.getInstance();
        AppConfiguration config2 = AppConfiguration.getInstance();
        System.out.println("Same instance? " + (config1 == config2)); // true

        System.out.println("App: " + config1.getAppName());
        System.out.println("DB URL: " + config1.getProperty("db.url"));

        // Enum singleton
        EnumSingleton.INSTANCE.setConfigValue("production");
        System.out.println("Config: " + EnumSingleton.INSTANCE.getConfigValue());

        // Bill Pugh
        BillPughSingleton s1 = BillPughSingleton.getInstance();
        BillPughSingleton s2 = BillPughSingleton.getInstance();
        System.out.println("Bill Pugh same? " + (s1 == s2)); // true
    }
}
```

| Approach | Thread-Safe | Lazy | Reflection-Safe | Best For |
|----------|-------------|------|-----------------|----------|
| Eager | ✅ | ❌ | ❌ | Simple, always-needed singletons |
| Synchronized | ✅ | ✅ | ❌ | Simple, low-contention |
| DCL | ✅ | ✅ | ❌ | High-performance multithreaded |
| Bill Pugh | ✅ | ✅ | ❌ | Most general use case |
| **Enum** | ✅ | ❌ | **✅** | When reflection/serialization safety matters |

### 🇻🇳 Tiếng Việt

**Singleton** đảm bảo chỉ có **một instance** của class trong suốt vòng đời ứng dụng.

**Các cách implement:**
1. **Eager**: Tạo ngay khi class được load — đơn giản, thread-safe
2. **Lazy + Synchronized**: Thread-safe nhưng chậm do lock mọi lần gọi
3. **Double-Checked Locking (DCL)**: Chỉ lock khi cần tạo instance — hiệu năng tốt
4. **Bill Pugh (Holder)**: Elegant nhất, dùng JVM class loading guarantee
5. **Enum Singleton**: Tốt nhất nếu cần chống reflection và serialization attack

**Khi nào dùng Singleton:**
- Configuration manager, Logger, Connection Pool, Cache

**Nhược điểm Singleton:**
- Khó unit test (global state)
- Coupling cao
- Vấn đề thread-safety nếu implement sai

**Thay thế hiện đại:** Dùng Dependency Injection (Spring `@Bean(scope=singleton)`) thay vì tự implement Singleton — dễ test và quản lý hơn.

---
## Q19. What is the hashCode() method in Java, and why is it important?

### 🇬🇧 English

`hashCode()` returns an integer that represents the object's "hash" — a fixed-size numeric summary of the object's content. It's critical for performance in hash-based collections like `HashMap`, `HashSet`, and `Hashtable`.

**The Contract (must always follow):**
1. If `a.equals(b)`, then `a.hashCode() == b.hashCode()`
2. Multiple calls to `hashCode()` on same unchanged object must return same value
3. If `!a.equals(b)`, `a.hashCode()` *may or may not* equal `b.hashCode()` (collisions allowed)

```java
// ============================================================
// hashCode() — Proper Implementation and Importance
// ============================================================

public class Student {
    private final String studentId;
    private final String name;
    private final String major;

    public Student(String studentId, String name, String major) {
        this.studentId = studentId;
        this.name = name;
        this.major = major;
    }

    @Override
    public boolean equals(Object o) {
        if (this == o) return true;
        if (!(o instanceof Student)) return false;
        Student other = (Student) o;
        return Objects.equals(studentId, other.studentId)
            && Objects.equals(name, other.name)
            && Objects.equals(major, other.major);
    }

    // CORRECT hashCode — uses same fields as equals()
    @Override
    public int hashCode() {
        return Objects.hash(studentId, name, major);
        // Objects.hash() combines multiple fields using prime multiplication:
        // result = 31 * (31 * field1.hashCode()) + field2.hashCode() + ...
    }

    // MANUAL implementation for learning:
    public int hashCodeManual() {
        int result = 17;                                     // Prime starting value
        result = 31 * result + (studentId != null ? studentId.hashCode() : 0);
        result = 31 * result + (name != null ? name.hashCode() : 0);
        result = 31 * result + (major != null ? major.hashCode() : 0);
        return result;
        // 31 is chosen because 31*n = (32*n - n) = (n<<5 - n) — fast bitwise op
    }

    @Override
    public String toString() {
        return "Student{id='" + studentId + "', name='" + name + "', major='" + major + "'}";
    }
}

public class HashCodeDemo {
    public static void main(String[] args) {
        Student s1 = new Student("S001", "Alice", "CS");
        Student s2 = new Student("S001", "Alice", "CS"); // Same content
        Student s3 = new Student("S002", "Bob", "Math");  // Different

        System.out.println("s1.equals(s2): " + s1.equals(s2)); // true
        System.out.println("s1.hashCode(): " + s1.hashCode());
        System.out.println("s2.hashCode(): " + s2.hashCode());
        System.out.println("Hashes equal: " + (s1.hashCode() == s2.hashCode())); // true

        // HashSet uses hashCode() to find the right bucket
        Set<Student> studentSet = new HashSet<>();
        studentSet.add(s1);
        studentSet.add(s2);  // Should be recognized as duplicate
        System.out.println("\nSet size (should be 1): " + studentSet.size()); // 1

        // HashMap lookup
        Map<Student, String> grades = new HashMap<>();
        grades.put(s1, "A+");
        // Lookup with s2 (same content, different object)
        System.out.println("Grade via s2: " + grades.get(s2)); // "A+" — works!
        System.out.println("Grade via s3: " + grades.get(s3)); // null

        // BROKEN hashCode demonstration (don't do this!)
        // If hashCode always returns same value:
        // - equals() still works correctly
        // - BUT HashMap degenerates to a linked list: O(1) → O(n)
    }
}
```

**How HashMap uses hashCode:**
```
put(key, value):
  1. hash = key.hashCode()
  2. bucketIndex = hash % buckets.length
  3. Store in that bucket's linked list/tree

get(key):
  1. hash = key.hashCode()
  2. bucketIndex = hash % buckets.length
  3. Walk bucket's list, compare using equals()
```

**Performance impact of bad hashCode:**
- `hashCode()` always returns 0 → O(1) becomes O(n) — catastrophic for large maps

### 🇻🇳 Tiếng Việt

`hashCode()` trả về một số nguyên đại diện cho "băm" của object — dùng để xác định **bucket** trong `HashMap`, `HashSet`.

**Cách HashMap hoạt động:**
1. Gọi `key.hashCode()` → tính index bucket
2. Đến bucket đó, dùng `equals()` tìm đúng key
3. Nếu `hashCode` tốt → O(1); nếu tất cả return cùng giá trị → O(n)

**Hợp đồng bắt buộc:**
- Nếu `a.equals(b)` = true → `a.hashCode()` **phải** bằng `b.hashCode()`
- Ngược lại không bắt buộc (hash collision được phép)

**Nguyên tắc:** Khi override `equals()`, **bắt buộc** override `hashCode()` sử dụng **cùng các fields**. Dùng `Objects.hash(field1, field2, ...)` để tránh tự tính toán.

---
## Q20. What is the difference between a mutable and an immutable object?

### 🇬🇧 English

| Aspect | Mutable Object | Immutable Object |
|--------|---------------|-----------------|
| **State** | Can change after creation | Cannot change after creation |
| **Thread safety** | Needs synchronization | Inherently thread-safe |
| **Examples** | `StringBuilder`, `ArrayList`, most POJOs | `String`, `Integer`, `LocalDate` |
| **Performance** | Better when frequently modified | Better when passed around safely |
| **Caching** | Cannot safely cache hash | Can cache hash (like String) |
| **Design** | Flexible | Safer, simpler |

```java
// ============================================================
// Mutable vs Immutable Objects
// ============================================================

// MUTABLE class — state can change
public class MutablePoint {
    private double x;
    private double y;

    public MutablePoint(double x, double y) {
        this.x = x;
        this.y = y;
    }

    // State can change via setters
    public void setX(double x) { this.x = x; }
    public void setY(double y) { this.y = y; }
    public double getX() { return x; }
    public double getY() { return y; }

    public void translate(double dx, double dy) {
        this.x += dx;
        this.y += dy;
    }
}

// IMMUTABLE class — state never changes after construction
// Recipe for immutability:
// 1. Declare class as final (prevent subclassing)
// 2. All fields private and final
// 3. No setters
// 4. Deep copy mutable fields in constructor
// 5. Return copies of mutable fields from getters
public final class ImmutablePoint {
    private final double x;  // final — cannot be reassigned
    private final double y;

    public ImmutablePoint(double x, double y) {
        this.x = x;
        this.y = y;
    }

    // Read-only accessors — no setters
    public double getX() { return x; }
    public double getY() { return y; }

    // Instead of mutating, return a NEW object
    public ImmutablePoint translate(double dx, double dy) {
        return new ImmutablePoint(x + dx, y + dy);
    }

    public ImmutablePoint scale(double factor) {
        return new ImmutablePoint(x * factor, y * factor);
    }

    public double distanceTo(ImmutablePoint other) {
        double dx = this.x - other.x;
        double dy = this.y - other.y;
        return Math.sqrt(dx * dx + dy * dy);
    }

    @Override
    public boolean equals(Object o) {
        if (this == o) return true;
        if (!(o instanceof ImmutablePoint)) return false;
        ImmutablePoint p = (ImmutablePoint) o;
        return Double.compare(x, p.x) == 0 && Double.compare(y, p.y) == 0;
    }

    @Override
    public int hashCode() {
        return Objects.hash(x, y);
    }

    @Override
    public String toString() { return "(" + x + ", " + y + ")"; }
}

// IMMUTABLE class with mutable fields — need deep copy
public final class ImmutableOrder {
    private final String orderId;
    private final List<String> items;  // List is mutable!
    private final java.time.LocalDate orderDate;

    public ImmutableOrder(String orderId, List<String> items, java.time.LocalDate date) {
        this.orderId = orderId;
        // Deep copy to prevent external modification
        this.items = List.copyOf(items);  // Unmodifiable copy (Java 10+)
        this.orderDate = date;  // LocalDate is already immutable
    }

    public String getOrderId() { return orderId; }
    public java.time.LocalDate getOrderDate() { return orderDate; }

    // Return unmodifiable view — prevents external mutation
    public List<String> getItems() {
        return Collections.unmodifiableList(items);
    }

    // "Wither" pattern — return modified copy
    public ImmutableOrder withNewItem(String item) {
        List<String> newItems = new ArrayList<>(items);
        newItems.add(item);
        return new ImmutableOrder(orderId, newItems, orderDate);
    }
}

public class MutableImmutableDemo {
    public static void main(String[] args) {
        // Mutable — be careful passing around
        MutablePoint mutable = new MutablePoint(3, 4);
        System.out.println("Before: " + mutable.getX() + ", " + mutable.getY());
        mutable.translate(1, 1);
        System.out.println("After translate: " + mutable.getX() + ", " + mutable.getY());

        // Immutable — safe to share
        ImmutablePoint p1 = new ImmutablePoint(3, 4);
        ImmutablePoint p2 = p1.translate(1, 1);  // New object, p1 unchanged
        System.out.println("p1: " + p1);  // (3.0, 4.0) — unchanged
        System.out.println("p2: " + p2);  // (4.0, 5.0) — new object

        // Thread safety: immutable objects can be shared freely
        ImmutablePoint shared = new ImmutablePoint(0, 0);
        // Multiple threads can read 'shared' without synchronization

        // Mutable requires synchronization
        // MutablePoint mutable2 = new MutablePoint(0, 0);
        // synchronized(mutable2) { mutable2.translate(1, 1); }

        // Immutable order
        List<String> initialItems = new ArrayList<>(Arrays.asList("Laptop", "Mouse"));
        ImmutableOrder order = new ImmutableOrder("ORD-001", initialItems, java.time.LocalDate.now());
        initialItems.add("Keyboard");  // Does NOT affect order! (deep copy)
        System.out.println("Order items: " + order.getItems()); // [Laptop, Mouse]

        ImmutableOrder updatedOrder = order.withNewItem("Keyboard");
        System.out.println("Updated: " + updatedOrder.getItems()); // [Laptop, Mouse, Keyboard]
        System.out.println("Original: " + order.getItems());       // [Laptop, Mouse] unchanged
    }
}
```

**Benefits of Immutability:**
- Thread-safe by nature — no synchronization needed
- Safe for caching and as HashMap keys
- Easier to reason about — no hidden state changes
- Defensive programming — cannot be tampered with

**Modern Java Tools for Immutability:**
```java
// Records (Java 16+) — immutable by default
record Coordinate(double lat, double lon) {}

// List.of(), Map.of() — immutable collections
List<String> list = List.of("a", "b", "c"); // Cannot add/remove

// String, Integer, LocalDate, BigDecimal — all immutable
```

### 🇻🇳 Tiếng Việt

**Mutable Object (Đối tượng có thể thay đổi):** Trạng thái có thể thay đổi sau khi tạo. Ví dụ: `StringBuilder`, `ArrayList`, hầu hết POJO.

**Immutable Object (Đối tượng bất biến):** Trạng thái không thể thay đổi sau khi tạo. Ví dụ: `String`, `Integer`, `LocalDate`.

**Cách tạo Immutable class:**
1. Khai báo class là `final`
2. Tất cả fields là `private final`
3. Không có setters
4. Deep copy mutable fields trong constructor
5. Return copy/unmodifiable view cho mutable fields

**Ưu điểm Immutable:**
- Thread-safe — không cần synchronized
- An toàn dùng làm HashMap key
- Dễ debug — không có side effects ẩn
- Thích hợp cho Value Objects (Money, Coordinate)

**Nhược điểm:** Tạo nhiều objects khi cần sửa đổi → tốn GC (nhưng JIT và GC hiện đại xử lý tốt)

---
# 🧹 PART 2: SOLID Principles and Clean Code

---
## Q21. What are the SOLID principles, and why are they important?

### 🇬🇧 English

**SOLID** is an acronym for five object-oriented design principles introduced by Robert C. Martin (Uncle Bob). They guide developers toward writing maintainable, flexible, and scalable code.

| Letter | Principle | One-Liner |
|--------|-----------|-----------|
| **S** | Single Responsibility | A class should have only one reason to change |
| **O** | Open/Closed | Open for extension, closed for modification |
| **L** | Liskov Substitution | Subtypes must be substitutable for their base types |
| **I** | Interface Segregation | Don't force clients to depend on interfaces they don't use |
| **D** | Dependency Inversion | Depend on abstractions, not concretions |

**Why are they important?**
- Reduce **coupling** — changes in one place don't ripple everywhere
- Increase **cohesion** — related code stays together
- Make code easier to **test** — small, focused classes/methods
- Support **extensibility** — add features without breaking existing code
- Enable **team scalability** — different developers work on different parts safely

```java
// Quick overview — all five principles in one example (Employee system)

// S — Single class for single responsibility
class EmployeeRepository { /* only handles data persistence */ }
class EmployeeSalaryCalculator { /* only handles salary logic */ }
class EmployeeReportGenerator { /* only handles report generation */ }

// O — Open for extension
interface TaxStrategy { double calculate(double salary); }
class StandardTax implements TaxStrategy { /* ... */ }
class SeniorTax implements TaxStrategy { /* ... */ }  // No modification to existing!

// L — Subtypes work everywhere base type works
class Employee { public double calculatePay() { return 0; } }
class FullTimeEmployee extends Employee { @Override public double calculatePay() { return 5000; } }
class PartTimeEmployee extends Employee { @Override public double calculatePay() { return 2500; } }
// Both can replace Employee reference safely

// I — Segregated interfaces
interface Payable { double calculatePay(); }
interface Reportable { String generateReport(); }
interface Manageable { void manage(Employee emp); }
// Classes only implement what they need

// D — Depend on abstractions
class PayrollService {
    private final Payable payable;  // Interface, not concrete class
    public PayrollService(Payable payable) { this.payable = payable; }
}
```

### 🇻🇳 Tiếng Việt

**SOLID** là bộ 5 nguyên tắc thiết kế hướng đối tượng giúp code dễ bảo trì, mở rộng và kiểm thử:

- **S** — Single Responsibility: Mỗi class chỉ có một lý do để thay đổi
- **O** — Open/Closed: Mở để mở rộng, đóng để sửa đổi
- **L** — Liskov Substitution: Lớp con phải thay thế được lớp cha mà không phá vỡ logic
- **I** — Interface Segregation: Không ép client phụ thuộc vào interface không cần thiết
- **D** — Dependency Inversion: Phụ thuộc vào abstraction, không phụ thuộc vào implementation cụ thể

**Tại sao quan trọng:** Giảm coupling, tăng cohesion → code dễ test, dễ mở rộng, ít bug khi thay đổi.

---
## Q22. Explain the Single Responsibility Principle (SRP) with an example.

### 🇬🇧 English

**SRP states:** A class should have **only one reason to change** — meaning it should have only one job or responsibility.

When a class handles multiple responsibilities, changing one aspect forces you to touch and potentially break other, unrelated functionality.

```java
// ============================================================
// SRP — Before and After Refactoring
// ============================================================

// ---- BEFORE: Violates SRP — Employee does too many things ----
// This class has MULTIPLE reasons to change:
// 1. Business logic changes (salary calculation)
// 2. Database schema changes (persistence)
// 3. Report format changes (reporting)
// 4. Email provider changes (notifications)
class Employee_BAD {
    private String name;
    private String email;
    private double baseSalary;
    private String department;

    // Responsibility 1: Business Logic
    public double calculateSalary() {
        double bonus = baseSalary * 0.1;
        double tax = baseSalary * 0.2;
        return baseSalary + bonus - tax;
    }

    // Responsibility 2: Data Persistence
    public void saveToDatabase() {
        // SQL logic mixed with business logic — BAD
        String sql = "INSERT INTO employees (name, email, salary) VALUES (?, ?, ?)";
        System.out.println("Executing: " + sql); // Simulated
        System.out.println("Employee saved to DB");
    }

    public static Employee_BAD loadFromDatabase(int id) {
        System.out.println("SELECT * FROM employees WHERE id=" + id);
        return new Employee_BAD(); // Simulated
    }

    // Responsibility 3: Reporting
    public String generateReport() {
        return String.format(
            "=== EMPLOYEE REPORT ===\nName: %s\nSalary: $%.2f\nDept: %s",
            name, calculateSalary(), department);
    }

    public void exportToPDF() {
        System.out.println("Generating PDF for " + name); // Heavy PDF logic
    }

    // Responsibility 4: Notifications
    public void sendWelcomeEmail() {
        System.out.println("Sending email to: " + email);
        // SMTP logic, template rendering, all mixed in here
    }
}

// ---- AFTER: Follows SRP — each class has ONE responsibility ----

// Responsibility 1: Pure data model (Entity)
public class Employee {
    private final int id;
    private String name;
    private String email;
    private double baseSalary;
    private String department;

    public Employee(int id, String name, String email, double baseSalary, String department) {
        this.id = id;
        this.name = name;
        this.email = email;
        this.baseSalary = baseSalary;
        this.department = department;
    }

    // Pure data accessors — no business logic, no I/O
    public int getId() { return id; }
    public String getName() { return name; }
    public String getEmail() { return email; }
    public double getBaseSalary() { return baseSalary; }
    public String getDepartment() { return department; }
    public void setBaseSalary(double salary) { this.baseSalary = salary; }
}

// Responsibility 2: Salary Calculation (only reason to change: tax/bonus policy)
public class SalaryCalculator {
    private static final double BONUS_RATE = 0.10;
    private static final double TAX_RATE = 0.20;

    public double calculate(Employee employee) {
        double gross = employee.getBaseSalary() * (1 + BONUS_RATE);
        double tax = employee.getBaseSalary() * TAX_RATE;
        return gross - tax;
    }

    public double calculateBonus(Employee employee) {
        return employee.getBaseSalary() * BONUS_RATE;
    }

    public double calculateTax(Employee employee) {
        return employee.getBaseSalary() * TAX_RATE;
    }
}

// Responsibility 3: Data Persistence (only reason to change: database/schema)
public class EmployeeRepository {
    private final Map<Integer, Employee> store = new HashMap<>();

    public void save(Employee employee) {
        store.put(employee.getId(), employee);
        System.out.println("Saved employee: " + employee.getName());
    }

    public Optional<Employee> findById(int id) {
        return Optional.ofNullable(store.get(id));
    }

    public List<Employee> findByDepartment(String department) {
        return store.values().stream()
            .filter(e -> department.equals(e.getDepartment()))
            .collect(java.util.stream.Collectors.toList());
    }

    public void delete(int id) {
        store.remove(id);
    }
}

// Responsibility 4: Reporting (only reason to change: report format/content)
public class EmployeeReportService {
    private final SalaryCalculator salaryCalc;

    public EmployeeReportService(SalaryCalculator salaryCalc) {
        this.salaryCalc = salaryCalc;
    }

    public String generateTextReport(Employee employee) {
        return String.format(
            "=== EMPLOYEE REPORT ===%n" +
            "Name:       %s%n" +
            "Department: %s%n" +
            "Base:       $%.2f%n" +
            "Net Salary: $%.2f%n",
            employee.getName(), employee.getDepartment(),
            employee.getBaseSalary(), salaryCalc.calculate(employee));
    }

    public String generateCSV(List<Employee> employees) {
        StringBuilder csv = new StringBuilder("ID,Name,Department,BaseSalary,NetSalary\n");
        for (Employee emp : employees) {
            csv.append(String.format("%d,%s,%s,%.2f,%.2f%n",
                emp.getId(), emp.getName(), emp.getDepartment(),
                emp.getBaseSalary(), salaryCalc.calculate(emp)));
        }
        return csv.toString();
    }
}

// Responsibility 5: Notifications (only reason to change: notification channel/template)
public class EmployeeNotificationService {
    private final String smtpHost;

    public EmployeeNotificationService(String smtpHost) {
        this.smtpHost = smtpHost;
    }

    public void sendWelcomeEmail(Employee employee) {
        String subject = "Welcome to the team, " + employee.getName() + "!";
        String body = String.format("Dear %s,\nWelcome aboard!\n\nBest regards,\nHR Team",
            employee.getName());
        sendEmail(employee.getEmail(), subject, body);
    }

    public void sendSalarySlip(Employee employee, double netSalary) {
        String subject = "Your salary slip";
        String body = String.format("Dear %s,\nYour net salary: $%.2f",
            employee.getName(), netSalary);
        sendEmail(employee.getEmail(), subject, body);
    }

    private void sendEmail(String to, String subject, String body) {
        System.out.printf("[SMTP:%s] To: %s | Subject: %s%n", smtpHost, to, subject);
    }
}

// Orchestration — bring it all together (still SRP — orchestration is its own job)
public class EmployeeService {
    private final EmployeeRepository repository;
    private final SalaryCalculator salaryCalc;
    private final EmployeeNotificationService notifier;
    private final EmployeeReportService reporter;

    public EmployeeService(EmployeeRepository repo, SalaryCalculator calc,
                           EmployeeNotificationService notifier, EmployeeReportService reporter) {
        this.repository = repo;
        this.salaryCalc = calc;
        this.notifier = notifier;
        this.reporter = reporter;
    }

    public Employee hire(String name, String email, double salary, String dept) {
        int id = (int)(Math.random() * 10000);
        Employee emp = new Employee(id, name, email, salary, dept);
        repository.save(emp);
        notifier.sendWelcomeEmail(emp);
        System.out.println("Hired: " + reporter.generateTextReport(emp));
        return emp;
    }

    public void processMonthlyPayroll() {
        // Process all employees — delegating to specialized classes
        System.out.println("Processing payroll...");
    }
}

public class SRPDemo {
    public static void main(String[] args) {
        EmployeeRepository repo = new EmployeeRepository();
        SalaryCalculator calc = new SalaryCalculator();
        EmployeeNotificationService notifier = new EmployeeNotificationService("smtp.company.com");
        EmployeeReportService reporter = new EmployeeReportService(calc);
        EmployeeService service = new EmployeeService(repo, calc, notifier, reporter);

        Employee alice = service.hire("Alice Johnson", "alice@co.com", 80_000, "Engineering");
        System.out.println("Net salary: $" + String.format("%.2f", calc.calculate(alice)));
        System.out.println(reporter.generateTextReport(alice));
    }
}
```

**Benefits of SRP:**
- Each class is small and focused → easier to understand and test
- Changes to one concern don't affect others
- Team members can work on different responsibilities independently

### 🇻🇳 Tiếng Việt

**Nguyên tắc Đơn nhiệm (SRP):** Mỗi class chỉ có **một lý do duy nhất để thay đổi** — nghĩa là chỉ có một nhiệm vụ duy nhất.

**Ví dụ vi phạm SRP:** Class `Employee_BAD` vừa tính lương, vừa lưu DB, vừa tạo báo cáo, vừa gửi email → 4 lý do để thay đổi.

**Sau khi refactor:**
- `Employee`: chỉ là data model
- `SalaryCalculator`: chỉ tính lương
- `EmployeeRepository`: chỉ xử lý persistence
- `EmployeeReportService`: chỉ tạo báo cáo
- `EmployeeNotificationService`: chỉ gửi thông báo

**Lợi ích:**
- Dễ test từng class độc lập
- Thay đổi format báo cáo → chỉ sửa `EmployeeReportService`, không ảnh hưởng tính lương
- Đổi database → chỉ sửa `EmployeeRepository`

---
## Q23. What is the Open/Closed Principle (OCP), and how does it improve code maintainability?

### 🇬🇧 English

**OCP states:** Software entities should be **open for extension** but **closed for modification**. You should be able to add new behavior without changing existing, tested code.

```java
// ============================================================
// OCP — Payment Processing Example
// ============================================================

// ---- BEFORE: Violates OCP ----
// Every time a new payment method is added, we MODIFY this class
// Risk: breaking existing payment methods
class PaymentProcessor_BAD {
    public void processPayment(String type, double amount) {
        if (type.equals("CREDIT_CARD")) {
            System.out.println("Processing credit card: $" + amount);
            // credit card specific logic...
        } else if (type.equals("PAYPAL")) {
            System.out.println("Processing PayPal: $" + amount);
            // PayPal logic...
        } else if (type.equals("BITCOIN")) {
            System.out.println("Processing Bitcoin: " + (amount / 45000) + " BTC");
            // Crypto logic...
        }
        // Adding new method = MODIFYING this class = violates OCP
    }
}

// ---- AFTER: Follows OCP ----
// Add new payment methods WITHOUT modifying existing code

// Abstraction — the "closed" part (don't modify this)
public interface PaymentMethod {
    PaymentResult process(PaymentRequest request);
    boolean supports(String paymentType);
    String getDescription();
}

public record PaymentRequest(String orderId, double amount, String currency, Map<String, String> metadata) {}
public record PaymentResult(boolean success, String transactionId, String message) {}

// Extension point 1 — Credit Card (add without modifying PaymentProcessor)
public class CreditCardPayment implements PaymentMethod {
    private final String gatewayUrl;

    public CreditCardPayment(String gatewayUrl) {
        this.gatewayUrl = gatewayUrl;
    }

    @Override
    public PaymentResult process(PaymentRequest request) {
        System.out.printf("[CreditCard] Processing $%.2f %s for order %s%n",
            request.amount(), request.currency(), request.orderId());
        // Real implementation: call credit card gateway API
        String txId = "CC-" + System.currentTimeMillis();
        return new PaymentResult(true, txId, "Credit card payment successful");
    }

    @Override
    public boolean supports(String paymentType) {
        return "CREDIT_CARD".equals(paymentType) || "DEBIT_CARD".equals(paymentType);
    }

    @Override
    public String getDescription() { return "Credit/Debit Card via " + gatewayUrl; }
}

// Extension point 2 — PayPal
public class PayPalPayment implements PaymentMethod {
    private final String clientId;

    public PayPalPayment(String clientId) { this.clientId = clientId; }

    @Override
    public PaymentResult process(PaymentRequest request) {
        System.out.printf("[PayPal] Processing $%.2f for order %s%n",
            request.amount(), request.orderId());
        String txId = "PP-" + System.currentTimeMillis();
        return new PaymentResult(true, txId, "PayPal payment successful");
    }

    @Override
    public boolean supports(String paymentType) { return "PAYPAL".equals(paymentType); }

    @Override
    public String getDescription() { return "PayPal (client: " + clientId + ")"; }
}

// Extension point 3 — Cryptocurrency (added LATER, no modification to existing code)
public class CryptoPayment implements PaymentMethod {
    private final String walletAddress;
    private final double btcPrice;

    public CryptoPayment(String walletAddress, double btcPrice) {
        this.walletAddress = walletAddress;
        this.btcPrice = btcPrice;
    }

    @Override
    public PaymentResult process(PaymentRequest request) {
        double btcAmount = request.amount() / btcPrice;
        System.out.printf("[Crypto] Processing %.8f BTC for order %s%n",
            btcAmount, request.orderId());
        String txId = "BTC-" + System.currentTimeMillis();
        return new PaymentResult(true, txId,
            String.format("Crypto payment: %.8f BTC sent to %s", btcAmount, walletAddress));
    }

    @Override
    public boolean supports(String paymentType) {
        return "BITCOIN".equals(paymentType) || "ETHEREUM".equals(paymentType);
    }

    @Override
    public String getDescription() { return "Crypto payment to " + walletAddress; }
}

// PaymentProcessor — CLOSED for modification, OPEN for extension
// Never needs to change when new payment methods are added
public class PaymentProcessor {
    private final List<PaymentMethod> paymentMethods = new ArrayList<>();

    public void registerPaymentMethod(PaymentMethod method) {
        paymentMethods.add(method);
        System.out.println("Registered: " + method.getDescription());
    }

    public PaymentResult processPayment(String type, PaymentRequest request) {
        return paymentMethods.stream()
            .filter(m -> m.supports(type))
            .findFirst()
            .map(m -> m.process(request))
            .orElse(new PaymentResult(false, null, "Unsupported payment type: " + type));
    }

    public List<String> getAvailableMethods() {
        return paymentMethods.stream()
            .map(PaymentMethod::getDescription)
            .collect(java.util.stream.Collectors.toList());
    }
}

public class OCPDemo {
    public static void main(String[] args) {
        PaymentProcessor processor = new PaymentProcessor();

        // Register payment methods — extending behavior without modifying PaymentProcessor
        processor.registerPaymentMethod(new CreditCardPayment("gateway.stripe.com"));
        processor.registerPaymentMethod(new PayPalPayment("client-abc-123"));
        processor.registerPaymentMethod(new CryptoPayment("1A2B3C4D", 45_000));

        // Process payments
        Map<String, String> meta = new HashMap<>();
        meta.put("cardLast4", "4242");

        PaymentRequest request = new PaymentRequest("ORD-001", 99.99, "USD", meta);

        PaymentResult r1 = processor.processPayment("CREDIT_CARD", request);
        System.out.println(r1.message());

        PaymentResult r2 = processor.processPayment("PAYPAL", request);
        System.out.println(r2.message());

        PaymentResult r3 = processor.processPayment("BITCOIN", request);
        System.out.println(r3.message());

        PaymentResult r4 = processor.processPayment("UNKNOWN", request);
        System.out.println(r4.message());  // Unsupported
    }
}
```

**How OCP improves maintainability:**
- New payment methods can be added by implementing an interface — no existing code changes
- Zero risk of breaking existing payment functionality
- Existing unit tests continue to pass
- Each implementation can be developed and deployed independently

### 🇻🇳 Tiếng Việt

**Nguyên tắc Mở/Đóng (OCP):** Code nên **mở để mở rộng** nhưng **đóng để sửa đổi**.

**Ví dụ vi phạm:** `PaymentProcessor_BAD` dùng `if/else` cho từng loại thanh toán → thêm phương thức mới phải **sửa** class này → nguy cơ phá vỡ logic hiện tại.

**Sau khi áp dụng OCP:** Định nghĩa interface `PaymentMethod`, mỗi loại thanh toán implement riêng. `PaymentProcessor` không bao giờ thay đổi — chỉ đăng ký thêm implementation mới.

**Áp dụng thực tế với Spring:**
```java
@Service
public class CryptoPayment implements PaymentMethod { ... }
// Spring tự detect và inject — không cần sửa PaymentProcessor
```

---
## Q24. How does the Liskov Substitution Principle (LSP) prevent design issues?

### 🇬🇧 English

**LSP states:** Objects of a superclass should be replaceable with objects of its subclasses without altering the correctness of the program. In other words, a subclass should behave like its parent everywhere the parent is used.

**Violations cause:** Unexpected behavior, runtime errors, broken contracts, code that must check `instanceof` everywhere.

```java
// ============================================================
// LSP — Shapes and Rectangle/Square Problem
// ============================================================

// ---- CLASSIC LSP VIOLATION: Square extends Rectangle ----
class Rectangle_BAD {
    protected int width;
    protected int height;

    public void setWidth(int w) { this.width = w; }
    public void setHeight(int h) { this.height = h; }
    public int getArea() { return width * height; }
}

class Square_BAD extends Rectangle_BAD {
    @Override
    public void setWidth(int w) {
        this.width = w;
        this.height = w;  // Square must keep sides equal
    }

    @Override
    public void setHeight(int h) {
        this.width = h;   // Square must keep sides equal
        this.height = h;
    }
}

// This code works for Rectangle but BREAKS for Square (LSP violation!)
public void testRectangle(Rectangle_BAD rect) {
    rect.setWidth(5);
    rect.setHeight(10);
    // For Rectangle: 5 * 10 = 50 ✓
    // For Square: 10 * 10 = 100 ✗ (setHeight changed width too!)
    assert rect.getArea() == 50 : "Expected 50, got " + rect.getArea();
    // This assertion FAILS for Square_BAD!
}

// ---- LSP-COMPLIANT DESIGN ----
// Use abstraction that both shapes can satisfy

// Abstract shape that doesn't make assumptions
public interface Shape {
    double area();
    double perimeter();
    String describe();
}

public class Rectangle implements Shape {
    private final double width;
    private final double height;

    public Rectangle(double width, double height) {
        if (width <= 0 || height <= 0) throw new IllegalArgumentException("Dimensions must be positive");
        this.width = width;
        this.height = height;
    }

    @Override
    public double area() { return width * height; }

    @Override
    public double perimeter() { return 2 * (width + height); }

    @Override
    public String describe() {
        return String.format("Rectangle(%.1f x %.1f)", width, height);
    }

    public double getWidth() { return width; }
    public double getHeight() { return height; }

    // Returns a new rectangle (immutable design)
    public Rectangle withWidth(double newWidth) {
        return new Rectangle(newWidth, height);
    }

    public Rectangle withHeight(double newHeight) {
        return new Rectangle(width, newHeight);
    }
}

public class Square implements Shape {
    private final double side;

    public Square(double side) {
        if (side <= 0) throw new IllegalArgumentException("Side must be positive");
        this.side = side;
    }

    @Override
    public double area() { return side * side; }

    @Override
    public double perimeter() { return 4 * side; }

    @Override
    public String describe() {
        return String.format("Square(%.1f x %.1f)", side, side);
    }

    public double getSide() { return side; }

    public Square withSide(double newSide) { return new Square(newSide); }
}

// ---- ANOTHER LSP EXAMPLE: Bird hierarchy ----
// VIOLATION: Penguin extends Bird but can't fly
abstract class Bird_BAD {
    public abstract void fly();  // Penguins can't fly! LSP violation
    public abstract String makeSound();
}

class Penguin_BAD extends Bird_BAD {
    @Override
    public void fly() {
        throw new UnsupportedOperationException("Penguins can't fly!"); // Breaks LSP!
    }

    @Override
    public String makeSound() { return "Squawk!"; }
}

// COMPLIANT DESIGN: Separate flying behavior
public interface Bird {
    String makeSound();
    String move();  // Generic movement
}

public interface FlyingBird extends Bird {
    void fly();
    int getMaxAltitude();
}

public class Eagle implements FlyingBird {
    @Override
    public String makeSound() { return "Screech!"; }

    @Override
    public String move() { return "Flying"; }

    @Override
    public void fly() { System.out.println("Eagle soaring at high altitude"); }

    @Override
    public int getMaxAltitude() { return 3000; }  // meters
}

public class Penguin implements Bird {
    @Override
    public String makeSound() { return "Squawk!"; }

    @Override
    public String move() { return "Swimming/Waddling"; }

    // No fly() — Penguin doesn't implement FlyingBird
}

// Code that ONLY needs Bird interface works with both
public void describeBird(Bird bird) {
    System.out.println("Sound: " + bird.makeSound());
    System.out.println("Moves by: " + bird.move());
}

// Code that needs flying works only with FlyingBird
public void makeItFly(FlyingBird bird) {
    bird.fly();
    System.out.println("Max altitude: " + bird.getMaxAltitude() + "m");
}

public class LSPDemo {
    public static void main(String[] args) {
        // All shapes substitutable through Shape interface
        Shape[] shapes = {
            new Rectangle(5, 10),
            new Square(7),
            new Rectangle(3, 3)
        };

        double totalArea = 0;
        for (Shape shape : shapes) {
            System.out.printf("%s — Area: %.1f, Perimeter: %.1f%n",
                shape.describe(), shape.area(), shape.perimeter());
            totalArea += shape.area();
        }
        System.out.println("Total area: " + totalArea);

        // Bird hierarchy
        Bird[] birds = {new Eagle(), new Penguin()};
        LSPDemo demo = new LSPDemo();
        for (Bird b : birds) {
            demo.describeBird(b);  // Works for BOTH
        }

        // Only Eagles can fly
        demo.makeItFly(new Eagle());
        // demo.makeItFly(new Penguin()); // Compile error! Penguin is not FlyingBird
    }
}
```

**LSP Checklist — Is your design LSP-compliant?**
- ✅ Subclass does not throw exceptions not thrown by parent
- ✅ Subclass does not strengthen preconditions
- ✅ Subclass does not weaken postconditions
- ✅ No `UnsupportedOperationException` thrown for inherited methods
- ✅ No `instanceof` checks needed in client code

### 🇻🇳 Tiếng Việt

**Nguyên tắc Thay thế Liskov (LSP):** Các đối tượng của lớp con phải có thể thay thế đối tượng lớp cha mà **không làm hỏng** logic chương trình.

**Vi phạm kinh điển:** `Square extends Rectangle` — khi set width của Square, height cũng thay đổi → code test Rectangle bị sai khi dùng Square.

**Cách fix:** Dùng abstraction chung (`Shape` interface) thay vì ép `Square` kế thừa từ `Rectangle`. Mỗi class implement theo đúng bản chất của mình.

**Dấu hiệu vi phạm LSP:**
- Lớp con throw `UnsupportedOperationException` cho phương thức kế thừa
- Client code phải dùng `instanceof` để check loại trước khi gọi
- Postcondition yếu hơn hoặc precondition mạnh hơn lớp cha

---
## Q25. What is the Interface Segregation Principle (ISP), and when should it be applied?

### 🇬🇧 English

**ISP states:** Clients should not be forced to depend on interfaces they do not use. Large, "fat" interfaces should be split into smaller, more specific ones.

```java
// ============================================================
// ISP — Worker/Robot Example
// ============================================================

// ---- BEFORE: FAT interface — ISP violation ----
interface Worker_BAD {
    void work();
    void eat();      // Robots don't eat — forced to implement!
    void sleep();    // Robots don't sleep — forced to implement!
    void takeBreak();
}

class HumanWorker implements Worker_BAD {
    @Override public void work() { System.out.println("Human working"); }
    @Override public void eat() { System.out.println("Human eating"); }
    @Override public void sleep() { System.out.println("Human sleeping"); }
    @Override public void takeBreak() { System.out.println("Human on break"); }
}

class RobotWorker implements Worker_BAD {
    @Override public void work() { System.out.println("Robot working"); }
    @Override public void eat() { throw new UnsupportedOperationException("Robots don't eat!"); }
    @Override public void sleep() { throw new UnsupportedOperationException("Robots don't sleep!"); }
    @Override public void takeBreak() { /* empty — robots don't take breaks */ }
}

// ---- AFTER: Segregated interfaces ----

// Focused interfaces — each represents one capability
public interface Workable {
    void work();
    WorkStatus getStatus();
}

public interface Eatable {
    void eat(String food);
    int getCaloriesConsumed();
}

public interface Sleepable {
    void sleep(int hours);
    boolean isRested();
}

public interface Rechargeable {
    void recharge(int minutes);
    int getBatteryLevel();
}

public enum WorkStatus { WORKING, IDLE, RESTING, OFFLINE }

// Human implements all biological capabilities
public class HumanEmployee implements Workable, Eatable, Sleepable {
    private String name;
    private WorkStatus status = WorkStatus.IDLE;
    private int caloriesConsumed = 0;
    private boolean rested = true;

    public HumanEmployee(String name) { this.name = name; }

    @Override
    public void work() {
        status = WorkStatus.WORKING;
        System.out.println(name + " is working...");
    }

    @Override
    public WorkStatus getStatus() { return status; }

    @Override
    public void eat(String food) {
        caloriesConsumed += 500;
        System.out.println(name + " eating " + food);
    }

    @Override
    public int getCaloriesConsumed() { return caloriesConsumed; }

    @Override
    public void sleep(int hours) {
        status = WorkStatus.RESTING;
        rested = true;
        System.out.println(name + " sleeping for " + hours + " hours");
    }

    @Override
    public boolean isRested() { return rested; }
}

// Robot implements only work and recharge capabilities
public class IndustrialRobot implements Workable, Rechargeable {
    private String model;
    private WorkStatus status = WorkStatus.IDLE;
    private int batteryLevel = 100;

    public IndustrialRobot(String model) { this.model = model; }

    @Override
    public void work() {
        if (batteryLevel < 10) {
            System.out.println(model + " needs recharging!");
            return;
        }
        batteryLevel -= 5;
        status = WorkStatus.WORKING;
        System.out.println(model + " working... (battery: " + batteryLevel + "%)");
    }

    @Override
    public WorkStatus getStatus() { return status; }

    @Override
    public void recharge(int minutes) {
        batteryLevel = Math.min(100, batteryLevel + minutes / 2);
        System.out.println(model + " recharging... (battery: " + batteryLevel + "%)");
    }

    @Override
    public int getBatteryLevel() { return batteryLevel; }
}

// Client code only depends on what it needs
public class WorkManager {
    // Only depends on Workable — doesn't care if worker is human or robot
    public void assignWork(List<Workable> workers) {
        workers.forEach(w -> {
            if (w.getStatus() != WorkStatus.WORKING) {
                w.work();
            }
        });
    }
}

public class CanteenManager {
    // Only depends on Eatable — robots never appear here
    public void serveLunch(List<Eatable> employees, String meal) {
        employees.forEach(e -> e.eat(meal));
    }
}

public class MaintenanceManager {
    // Only depends on Rechargeable — humans never appear here
    public void chargeRobots(List<Rechargeable> robots) {
        robots.forEach(r -> {
            if (r.getBatteryLevel() < 20) {
                r.recharge(60);
            }
        });
    }
}

public class ISPDemo {
    public static void main(String[] args) {
        HumanEmployee alice = new HumanEmployee("Alice");
        HumanEmployee bob = new HumanEmployee("Bob");
        IndustrialRobot robot1 = new IndustrialRobot("ARM-X1");
        IndustrialRobot robot2 = new IndustrialRobot("WELD-Y2");

        WorkManager workMgr = new WorkManager();
        workMgr.assignWork(Arrays.asList(alice, bob, robot1, robot2)); // Works for all!

        CanteenManager canteen = new CanteenManager();
        canteen.serveLunch(Arrays.asList(alice, bob), "Pizza"); // Only humans

        MaintenanceManager maintenance = new MaintenanceManager();
        maintenance.chargeRobots(Arrays.asList(robot1, robot2)); // Only robots
    }
}
```

**When to apply ISP:**
- When an interface is growing too large (more than 5-7 methods)
- When implementing classes often have to leave methods empty or throw exceptions
- When different clients use different subsets of an interface

### 🇻🇳 Tiếng Việt

**Nguyên tắc Phân tách Interface (ISP):** Client không nên bị ép phụ thuộc vào interface mà nó không dùng.

**Vi phạm:** Interface `Worker_BAD` có `eat()` và `sleep()` nhưng Robot phải implement và throw exception — vô lý.

**Sau khi refactor:** Tách thành các interface nhỏ: `Workable`, `Eatable`, `Sleepable`, `Rechargeable`. Mỗi class chỉ implement những gì nó thực sự cần.

**Dấu hiệu cần áp dụng ISP:**
- Interface quá nhiều phương thức (fat interface)
- Các class implement phải để trống hoặc throw `UnsupportedOperationException`
- Các client chỉ dùng một phần nhỏ của interface

---
## Q26. Explain the Dependency Inversion Principle (DIP) with a real-world example.

### 🇬🇧 English

**DIP states:**
1. High-level modules should not depend on low-level modules. Both should depend on abstractions.
2. Abstractions should not depend on details. Details should depend on abstractions.

```java
// ============================================================
// DIP — Order Processing System
// ============================================================

// ---- BEFORE: Violates DIP ----
// High-level OrderService directly depends on low-level MySQL and SMTP
class MySQLOrderRepository {
    public void save(String order) {
        System.out.println("Saving to MySQL: " + order);
    }
    public String findById(int id) { return "Order-" + id; }
}

class SmtpEmailService {
    public void sendEmail(String to, String message) {
        System.out.println("SMTP Email to " + to + ": " + message);
    }
}

class OrderService_BAD {
    // Tight coupling to SPECIFIC implementations
    private MySQLOrderRepository mysqlRepo = new MySQLOrderRepository(); // Hard dependency!
    private SmtpEmailService emailService = new SmtpEmailService();       // Hard dependency!

    public void placeOrder(String customerId, String productId, int qty) {
        String order = customerId + ":" + productId + ":" + qty;
        mysqlRepo.save(order);   // Cannot switch to PostgreSQL without changing this class
        emailService.sendEmail(customerId + "@example.com", "Your order: " + order);
        // Cannot switch to SendGrid without changing this class
    }
}

// ---- AFTER: Follows DIP ----

// ABSTRACTIONS — both high-level and low-level depend on these
public interface OrderRepository {
    void save(Order order);
    Optional<Order> findById(String orderId);
    List<Order> findByCustomerId(String customerId);
}

public interface NotificationService {
    void sendOrderConfirmation(String customerId, Order order);
    void sendShippingUpdate(String customerId, Order order, String trackingNumber);
}

public interface PaymentGateway {
    PaymentResult charge(String customerId, double amount, String currency);
    boolean refund(String transactionId, double amount);
}

// DATA MODEL
public class Order {
    private final String orderId;
    private final String customerId;
    private final List<OrderLineItem> items;
    private OrderStatus status;
    private final java.time.LocalDateTime createdAt;

    public Order(String customerId, List<OrderLineItem> items) {
        this.orderId = "ORD-" + System.currentTimeMillis();
        this.customerId = customerId;
        this.items = new ArrayList<>(items);
        this.status = OrderStatus.PENDING;
        this.createdAt = java.time.LocalDateTime.now();
    }

    public double getTotal() {
        return items.stream().mapToDouble(i -> i.price() * i.quantity()).sum();
    }

    public String getOrderId() { return orderId; }
    public String getCustomerId() { return customerId; }
    public OrderStatus getStatus() { return status; }
    public void setStatus(OrderStatus status) { this.status = status; }
}

public record OrderLineItem(String productId, String name, double price, int quantity) {}
public enum OrderStatus { PENDING, CONFIRMED, SHIPPED, DELIVERED, CANCELLED }

// LOW-LEVEL MODULES — details that depend on abstractions
public class MySQLOrderRepository2 implements OrderRepository {
    private final String connectionString;

    public MySQLOrderRepository2(String connectionString) {
        this.connectionString = connectionString;
    }

    @Override
    public void save(Order order) {
        System.out.println("[MySQL] Saving order: " + order.getOrderId());
        // Real implementation: execute INSERT SQL
    }

    @Override
    public Optional<Order> findById(String orderId) {
        System.out.println("[MySQL] Finding order: " + orderId);
        return Optional.empty(); // Simulated
    }

    @Override
    public List<Order> findByCustomerId(String customerId) { return new ArrayList<>(); }
}

// Can swap to PostgreSQL without changing OrderService!
public class PostgreSQLOrderRepository implements OrderRepository {
    @Override
    public void save(Order order) {
        System.out.println("[PostgreSQL] Saving order: " + order.getOrderId());
    }
    @Override public Optional<Order> findById(String id) { return Optional.empty(); }
    @Override public List<Order> findByCustomerId(String id) { return new ArrayList<>(); }
}

public class EmailNotificationService implements NotificationService {
    private final String smtpHost;

    public EmailNotificationService(String smtpHost) { this.smtpHost = smtpHost; }

    @Override
    public void sendOrderConfirmation(String customerId, Order order) {
        System.out.printf("[SMTP:%s] Order confirmation for %s: order %s ($%.2f)%n",
            smtpHost, customerId, order.getOrderId(), order.getTotal());
    }

    @Override
    public void sendShippingUpdate(String customerId, Order order, String tracking) {
        System.out.printf("[SMTP:%s] Shipping update for %s: tracking %s%n",
            smtpHost, customerId, tracking);
    }
}

// Can swap to SMS without changing OrderService!
public class SmsNotificationService implements NotificationService {
    @Override
    public void sendOrderConfirmation(String customerId, Order order) {
        System.out.printf("[SMS] Order %s confirmed for %s%n", order.getOrderId(), customerId);
    }

    @Override
    public void sendShippingUpdate(String customerId, Order order, String tracking) {
        System.out.printf("[SMS] Your order %s shipped. Track: %s%n",
            order.getOrderId(), tracking);
    }
}

// HIGH-LEVEL MODULE — depends only on abstractions (interfaces)
// DIP-compliant: never mentions MySQL, PostgreSQL, SMTP, SMS
public class OrderService {
    private final OrderRepository orderRepository;        // Abstraction, not MySQL
    private final NotificationService notificationService; // Abstraction, not SMTP
    private final PaymentGateway paymentGateway;           // Abstraction

    // Dependencies INJECTED through constructor (Dependency Injection)
    public OrderService(OrderRepository orderRepository,
                        NotificationService notificationService,
                        PaymentGateway paymentGateway) {
        this.orderRepository = orderRepository;
        this.notificationService = notificationService;
        this.paymentGateway = paymentGateway;
    }

    public Order placeOrder(String customerId, List<OrderLineItem> items) {
        Order order = new Order(customerId, items);

        // Business logic — high-level
        PaymentResult payment = paymentGateway.charge(customerId, order.getTotal(), "USD");
        if (!payment.success()) {
            throw new RuntimeException("Payment failed: " + payment.message());
        }

        order.setStatus(OrderStatus.CONFIRMED);
        orderRepository.save(order);
        notificationService.sendOrderConfirmation(customerId, order);

        System.out.println("Order placed: " + order.getOrderId());
        return order;
    }

    public void shipOrder(String orderId, String trackingNumber) {
        orderRepository.findById(orderId).ifPresent(order -> {
            order.setStatus(OrderStatus.SHIPPED);
            orderRepository.save(order);
            notificationService.sendShippingUpdate(order.getCustomerId(), order, trackingNumber);
        });
    }
}

public class DIPDemo {
    public static void main(String[] args) {
        // Composition Root — wire up dependencies
        // For production: MySQL + Email
        OrderRepository prodRepo = new MySQLOrderRepository2("jdbc:mysql://localhost/orders");
        NotificationService emailNotifier = new EmailNotificationService("smtp.company.com");
        PaymentGateway stripeGateway = (custId, amount, currency) ->
            new PaymentResult(true, "txn-" + System.currentTimeMillis(), "Charged via Stripe");

        OrderService orderService = new OrderService(prodRepo, emailNotifier, stripeGateway);

        List<OrderLineItem> items = List.of(
            new OrderLineItem("P001", "Laptop", 999.99, 1),
            new OrderLineItem("P002", "Mouse", 29.99, 2)
        );
        orderService.placeOrder("CUST-001", items);

        // For testing: InMemory + Mock notifications (no infrastructure needed!)
        OrderRepository testRepo = new InMemoryOrderRepository(); // Test double
        NotificationService mockNotifier = (custId, order) ->
            System.out.println("[TEST] Notification sent"); // Lambda for test
        // ... etc
    }
}

// Simple in-memory repository for testing
class InMemoryOrderRepository implements OrderRepository {
    private final Map<String, Order> store = new HashMap<>();

    @Override public void save(Order order) { store.put(order.getOrderId(), order); }
    @Override public Optional<Order> findById(String id) { return Optional.ofNullable(store.get(id)); }
    @Override public List<Order> findByCustomerId(String cid) {
        return store.values().stream()
            .filter(o -> o.getCustomerId().equals(cid))
            .collect(java.util.stream.Collectors.toList());
    }
}
```

### 🇻🇳 Tiếng Việt

**Nguyên tắc Đảo ngược Phụ thuộc (DIP):**
1. Module cấp cao không phụ thuộc vào module cấp thấp — cả hai phụ thuộc vào abstraction
2. Abstraction không phụ thuộc vào detail — detail phụ thuộc vào abstraction

**Vi phạm:** `OrderService_BAD` tạo trực tiếp `new MySQLOrderRepository()` — khi muốn đổi sang PostgreSQL phải sửa `OrderService`.

**Sau khi áp dụng DIP:** `OrderService` nhận interface `OrderRepository`, `NotificationService` qua constructor injection. Để đổi database → chỉ cần tạo implementation mới và inject vào.

**Lợi ích:**
- Dễ test: inject mock/stub trong unit test
- Dễ thay thế implementation: MySQL → PostgreSQL, SMTP → SendGrid
- Code business logic không phụ thuộc vào infrastructure

---
## Q27. What are the best practices for writing clean and maintainable code?

### 🇬🇧 English

Clean code is code that is **easy to read, understand, and modify**. It communicates intent clearly, without needing excessive comments.

```java
// ============================================================
// Clean Code Principles — Before and After
// ============================================================

// ---- BAD: Hard to understand ----
public List<int[]> getThem(List<int[]> lst) {
    List<int[]> res = new ArrayList<>();
    for (int[] x : lst) {
        if (x[0] == 4) res.add(x);
    }
    return res;
}
// What does this do? What is 4? What is x[0]?

// ---- GOOD: Self-documenting ----
public static final int STATUS_FLAGGED = 4;

public List<int[]> getFlaggedCells(List<int[]> gameBoard) {
    List<int[]> flaggedCells = new ArrayList<>();
    for (int[] cell : gameBoard) {
        if (isFlagged(cell)) {
            flaggedCells.add(cell);
        }
    }
    return flaggedCells;
}

private boolean isFlagged(int[] cell) {
    return cell[GameCell.STATUS_INDEX] == STATUS_FLAGGED;
}

// ---- Clean Code Principles Demonstrated ----

// 1. MEANINGFUL NAMES
// BAD:
int d; // elapsed time in days
// GOOD:
int elapsedTimeInDays;

// 2. SMALL FUNCTIONS WITH ONE JOB
// BAD: One giant method doing everything
public void processUserRegistration_BAD(String name, String email,
                                         String password, String role) {
    // Validate
    if (name == null || name.length() < 2) throw new IllegalArgumentException("bad name");
    if (!email.contains("@")) throw new IllegalArgumentException("bad email");
    if (password.length() < 8) throw new IllegalArgumentException("bad pass");

    // Hash password
    String hash = "";
    for (int i = 0; i < password.length(); i++) hash += (int)password.charAt(i);

    // Save to DB
    System.out.println("INSERT INTO users (name, email, password_hash, role) VALUES (...)");

    // Send email
    System.out.println("Sending welcome email to " + email);

    // Log
    System.out.println("User registered: " + email);
}

// GOOD: Each method does one thing
public class UserRegistrationService {
    private final UserValidator validator;
    private final PasswordEncoder passwordEncoder;
    private final UserRepository userRepository;
    private final EmailService emailService;

    public UserRegistrationService(UserValidator validator, PasswordEncoder passwordEncoder,
                                   UserRepository userRepository, EmailService emailService) {
        this.validator = validator;
        this.passwordEncoder = passwordEncoder;
        this.userRepository = userRepository;
        this.emailService = emailService;
    }

    public User registerUser(UserRegistrationRequest request) {
        validator.validate(request);
        String encodedPassword = passwordEncoder.encode(request.password());
        User user = createUser(request, encodedPassword);
        User savedUser = userRepository.save(user);
        emailService.sendWelcomeEmail(savedUser);
        return savedUser;
    }

    private User createUser(UserRegistrationRequest request, String encodedPassword) {
        return new User(request.name(), request.email(), encodedPassword, request.role());
    }
}

// 3. AVOID MAGIC NUMBERS — use named constants
// BAD:
if (age >= 18 && attempts < 3 && score > 600) { /* ... */ }

// GOOD:
private static final int LEGAL_AGE = 18;
private static final int MAX_LOGIN_ATTEMPTS = 3;
private static final int MIN_CREDIT_SCORE = 600;

if (age >= LEGAL_AGE && attempts < MAX_LOGIN_ATTEMPTS && score > MIN_CREDIT_SCORE) { /* ... */ }

// 4. GUARD CLAUSES — reduce nesting
// BAD: deep nesting
public String processOrder_BAD(Order order) {
    if (order != null) {
        if (order.getCustomerId() != null) {
            if (!order.getItems().isEmpty()) {
                if (order.getTotal() > 0) {
                    return "Order processed: " + order.getOrderId();
                }
            }
        }
    }
    return null;
}

// GOOD: Guard clauses (early returns)
public String processOrder(Order order) {
    if (order == null) return null;
    if (order.getCustomerId() == null) throw new IllegalArgumentException("No customer");
    if (order.getItems().isEmpty()) throw new IllegalArgumentException("No items");
    if (order.getTotal() <= 0) throw new IllegalArgumentException("Invalid total");

    return "Order processed: " + order.getOrderId();
}

// 5. AVOID COMMENTS — write self-documenting code
// BAD: comment explains what (the code already does that)
// Increment i
i++;

// BAD: comment explains unclear code
// Check if employee is eligible for full benefits
if ((employee.flags & HOURLY_FLAG) && employee.age > 65) { }

// GOOD: meaningful name
if (employee.isEligibleForFullBenefits()) { }

// Comments ARE good for: WHY, not WHAT
// Using MD5 is intentional — this system requires compatibility with legacy clients
// See: https://legacy-docs.example.com/auth-spec
String hash = md5(password);

// 6. DON'T RETURN NULL — use Optional
// BAD:
public User findUser_BAD(String id) {
    // ... returns null if not found
    return null; // Callers forget to check for null → NullPointerException
}

// GOOD:
public Optional<User> findUser(String id) {
    // Callers are FORCED to handle the missing case
    return Optional.ofNullable(store.get(id));
}
// Usage:
// findUser("123").ifPresent(user -> sendEmail(user));
// String name = findUser("123").map(User::getName).orElse("Unknown");
```

**Clean Code Checklist:**
- [ ] Names reveal intent
- [ ] Functions do one thing
- [ ] No magic numbers/strings
- [ ] Guard clauses replace deep nesting
- [ ] No duplicate code (DRY)
- [ ] Errors handled explicitly
- [ ] Tests pass and are readable

### 🇻🇳 Tiếng Việt

**Code sạch (Clean Code)** là code dễ đọc, dễ hiểu, dễ thay đổi — không cần comment nhiều vì code tự nói lên ý nghĩa.

**Các nguyên tắc chính:**

1. **Đặt tên có ý nghĩa:** `elapsedTimeInDays` thay vì `d`; `getFlaggedCells()` thay vì `getThem()`
2. **Hàm nhỏ, một việc:** Mỗi function chỉ làm một việc, đặt tên động từ rõ ràng
3. **Tránh magic numbers:** Dùng hằng số `MAX_LOGIN_ATTEMPTS = 3` thay vì số `3` rải rác
4. **Guard clauses:** Early return thay vì lồng `if` sâu
5. **Tránh null:** Dùng `Optional<T>` để buộc caller xử lý trường hợp không có giá trị
6. **Comment WHY, không comment WHAT:** Code tự giải thích what, comment giải thích why

---
## Q28. How do code smells impact software maintainability?

### 🇬🇧 English

**Code smells** are indicators of deeper problems in the code — not bugs per se, but patterns that suggest the design is flawed and will become hard to maintain.

**Common Code Smells and Fixes:**

```java
// ============================================================
// Code Smells — Identification and Fixes
// ============================================================

// SMELL 1: LONG METHOD — method does too much
// BAD:
public void processMonthlyPayroll_BAD(List<Employee> employees) {
    // 200 lines of: calculate salary, deductions, taxes, bonuses,
    // save to DB, generate pay stubs, send emails, update HR system...
}

// FIX: Extract methods
public void processMonthlyPayroll(List<Employee> employees) {
    List<PayrollRecord> records = calculatePayroll(employees);
    savePayrollRecords(records);
    generatePayStubs(records);
    sendPaymentNotifications(records);
    updateHRSystem(records);
}

// SMELL 2: LARGE CLASS (God Object) — class knows too much
// BAD: OrderManager with 50+ fields and 100+ methods
// FIX: Split responsibilities using SRP (see Q22)

// SMELL 3: FEATURE ENVY — method uses another class's data more than its own
// BAD: Order method manipulates Customer data extensively
class Order_SmellDemo {
    private Customer customer;
    private List<Item> items;

    // FEATURE ENVY: This method envies Customer class
    public double calculateDiscount_BAD() {
        double discount = 0;
        if (customer.getLoyaltyPoints() > 1000) discount += 0.10;
        if (customer.getMembershipLevel().equals("GOLD")) discount += 0.05;
        if (customer.getPurchaseHistory().size() > 10) discount += 0.03;
        return discount;
    }
}

// FIX: Move method to where the data lives
class Customer {
    private int loyaltyPoints;
    private String membershipLevel;
    private List<String> purchaseHistory;

    // Method belongs HERE — uses Customer's own data
    public double calculateDiscount() {
        double discount = 0;
        if (loyaltyPoints > 1000) discount += 0.10;
        if ("GOLD".equals(membershipLevel)) discount += 0.05;
        if (purchaseHistory.size() > 10) discount += 0.03;
        return discount;
    }

    public int getLoyaltyPoints() { return loyaltyPoints; }
    public String getMembershipLevel() { return membershipLevel; }
    public List<String> getPurchaseHistory() { return purchaseHistory; }
}

// SMELL 4: DATA CLUMPS — same group of variables always appear together
// BAD: Everywhere you see (String street, String city, String country, String zip)
public void createUser_BAD(String name, String street, String city,
                            String country, String zip, String phone) { }
public void updateAddress_BAD(int userId, String street, String city,
                               String country, String zip) { }

// FIX: Introduce Parameter Object
record Address(String street, String city, String country, String zip) {}
record PhoneNumber(String countryCode, String number) {}

public void createUser(String name, Address address, PhoneNumber phone) { }
public void updateAddress(int userId, Address address) { }

// SMELL 5: PRIMITIVE OBSESSION — using primitives where objects should be
// BAD:
public class Order2 {
    private double price;  // Is it USD? EUR? Can be negative?
    private String status; // Any string can be passed — typos possible
    private String customerId; // String vs typed ID
}

// FIX: Replace primitives with value objects and enums
record Money(double amount, String currency) {
    public Money {
        if (amount < 0) throw new IllegalArgumentException("Amount cannot be negative");
        if (currency == null) throw new IllegalArgumentException("Currency required");
    }
}
enum OrderStatus2 { PENDING, CONFIRMED, SHIPPED, DELIVERED }
record CustomerId(String value) {
    public CustomerId {
        if (value == null || !value.matches("CUST-\\d+"))
            throw new IllegalArgumentException("Invalid customer ID: " + value);
    }
}

// SMELL 6: SWITCH STATEMENTS — often a sign missing polymorphism
// BAD: switch scattered across codebase
public double calculateShipping_BAD(String method, double weight) {
    switch (method) {
        case "STANDARD": return weight * 0.5;
        case "EXPRESS": return weight * 1.5;
        case "OVERNIGHT": return weight * 3.0;
        default: throw new IllegalArgumentException("Unknown method: " + method);
    }
}

// FIX: Polymorphism
interface ShippingMethod {
    double calculateCost(double weight);
    String getName();
}

class StandardShipping implements ShippingMethod {
    @Override public double calculateCost(double weight) { return weight * 0.5; }
    @Override public String getName() { return "Standard"; }
}

class ExpressShipping implements ShippingMethod {
    @Override public double calculateCost(double weight) { return weight * 1.5; }
    @Override public String getName() { return "Express"; }
}

// SMELL 7: DUPLICATED CODE
// BAD: Same validation logic in UserService and AdminService
// FIX: Extract to shared EmailValidator class

public class EmailValidator {
    private static final String EMAIL_PATTERN = "^[A-Za-z0-9+_.-]+@[A-Za-z0-9.-]+\\.[A-Za-z]{2,}$";

    public static boolean isValid(String email) {
        return email != null && email.matches(EMAIL_PATTERN);
    }

    public static void validate(String email) {
        if (!isValid(email)) throw new IllegalArgumentException("Invalid email: " + email);
    }
}

// SMELL 8: COMMENTS EXPLAINING BAD CODE
// BAD: Comment explains what confusing code does
// j is the index, a is the array, we iterate backwards for some reason
for (int j = a.length - 1; j >= 0; j--) { /* ... */ }

// FIX: Write clear code that doesn't need a comment
for (int index = lastIndex; index >= FIRST_INDEX; index--) { /* ... */ }
```

**Code Smell Quick Reference:**

| Smell | Symptom | Fix |
|-------|---------|-----|
| Long Method | Method > 20 lines | Extract Method |
| Large Class | Class > 300 lines | Extract Class |
| Feature Envy | Method touches other class's data | Move Method |
| Data Clumps | Same params grouped always | Introduce Parameter Object |
| Primitive Obsession | Using String/int where class needed | Replace with Value Object |
| Switch Statements | Type-checking switches | Polymorphism |
| Duplicate Code | Copy-paste code | Extract common logic |
| Dead Code | Unused variables/methods | Delete it |

### 🇻🇳 Tiếng Việt

**Code smell** là các dấu hiệu cho thấy thiết kế code có vấn đề — không phải bug trực tiếp, nhưng sẽ gây khó khăn khi bảo trì, mở rộng và kiểm thử.

**Các code smell phổ biến:**
- **Long Method**: Method quá dài → Extract Method
- **Large Class (God Object)**: Class quá nhiều việc → Split bằng SRP
- **Feature Envy**: Method dùng data của class khác nhiều hơn của mình → Move Method
- **Data Clumps**: Các tham số luôn đi cùng nhau → Tạo Parameter Object
- **Primitive Obsession**: Dùng `String` cho status, tiền tệ, email → Value Object
- **Duplicate Code**: Copy-paste logic → Extract thành shared class/method

**Tác hại:** Code smells tích tụ dẫn đến "technical debt" — càng để lâu càng khó sửa, tăng chi phí bảo trì, tăng nguy cơ bug.

---
## Q29. What are some common refactoring techniques to improve code quality?

### 🇬🇧 English

**Refactoring** is the process of improving code structure without changing its external behavior. It eliminates technical debt incrementally.

```java
// ============================================================
// Refactoring Techniques
// ============================================================

// TECHNIQUE 1: EXTRACT METHOD
// Before:
public void printOwing_BAD() {
    double outstanding = 0;
    // Print banner
    System.out.println("*************************");
    System.out.println("***** Customer Owes *****");
    System.out.println("*************************");
    // Calculate outstanding
    for (Order order : orders) {
        outstanding += order.getTotal();
    }
    // Print details
    System.out.println("name: " + customer.getName());
    System.out.println("amount: " + outstanding);
}

// After:
public void printOwing() {
    printBanner();
    double outstanding = calculateOutstanding();
    printDetails(outstanding);
}

private void printBanner() {
    System.out.println("*************************");
    System.out.println("***** Customer Owes *****");
    System.out.println("*************************");
}

private double calculateOutstanding() {
    return orders.stream().mapToDouble(Order::getTotal).sum();
}

private void printDetails(double outstanding) {
    System.out.println("name: " + customer.getName());
    System.out.println("amount: " + outstanding);
}

// TECHNIQUE 2: REPLACE TEMP WITH QUERY
// Before:
public double getPrice_BAD() {
    double basePrice = quantity * itemPrice;
    double discountFactor;
    if (basePrice > 1000) discountFactor = 0.95;
    else discountFactor = 0.98;
    return basePrice * discountFactor;
}

// After: temp variables replaced with methods
public double getPrice() {
    return basePrice() * discountFactor();
}

private double basePrice() { return quantity * itemPrice; }

private double discountFactor() {
    return basePrice() > 1000 ? 0.95 : 0.98;
}

// TECHNIQUE 3: INTRODUCE PARAMETER OBJECT
// Before: data clump
public void amountInvoiced_BAD(java.util.Date start, java.util.Date end) { }
public void amountReceived_BAD(java.util.Date start, java.util.Date end) { }

// After: DateRange encapsulates the pair
record DateRange(java.time.LocalDate start, java.time.LocalDate end) {
    public DateRange {
        if (start.isAfter(end)) throw new IllegalArgumentException("Start must be before end");
    }
    public boolean includes(java.time.LocalDate date) {
        return !date.isBefore(start) && !date.isAfter(end);
    }
}

public void amountInvoiced(DateRange range) { }
public void amountReceived(DateRange range) { }

// TECHNIQUE 4: REPLACE CONDITIONAL WITH POLYMORPHISM
// Before:
public double getSpeed_BAD(String type) {
    switch (type) {
        case "EUROPEAN": return 35.0;
        case "AFRICAN": return isCoconutLoaded ? 25.0 : 40.0;
        case "NORWEGIAN_BLUE": return voltage > 100 ? 18.0 : 12.0;
        default: throw new IllegalArgumentException("Unknown bird: " + type);
    }
}

// After: each type has its own behavior
interface Bird2 { double getSpeed(); }

class EuropeanSwallow implements Bird2 {
    @Override public double getSpeed() { return 35.0; }
}

class AfricanSwallow implements Bird2 {
    private boolean coconutLoaded;
    public AfricanSwallow(boolean coconutLoaded) { this.coconutLoaded = coconutLoaded; }
    @Override public double getSpeed() { return coconutLoaded ? 25.0 : 40.0; }
}

class NorwegianBlueParrot implements Bird2 {
    private double voltage;
    public NorwegianBlueParrot(double voltage) { this.voltage = voltage; }
    @Override public double getSpeed() { return voltage > 100 ? 18.0 : 12.0; }
}

// TECHNIQUE 5: ENCAPSULATE FIELD
// Before: public field
class Person_BAD {
    public String name;
}

// After: private field + getter/setter with validation
class Person_Good {
    private String name;

    public String getName() { return name; }
    public void setName(String name) {
        if (name == null || name.isBlank())
            throw new IllegalArgumentException("Name cannot be blank");
        this.name = name.trim();
    }
}

// TECHNIQUE 6: REPLACE MAGIC NUMBER WITH SYMBOLIC CONSTANT
// Before:
double potential = quantity * 0.00087; // What is 0.00087?

// After:
static final double CONVERSION_FACTOR = 0.00087;  // Document what it means
double potential = quantity * CONVERSION_FACTOR;

// TECHNIQUE 7: DECOMPOSE CONDITIONAL
// Before:
if (!aDate.isBefore(SUMMER_START) && !aDate.isAfter(SUMMER_END)) {
    charge = quantity * summerRate + summerServiceCharge;
} else {
    charge = quantity * regularRate + regularServiceCharge;
}

// After:
if (isSummer(aDate)) {
    charge = summerCharge(quantity);
} else {
    charge = regularCharge(quantity);
}
```

**Safe Refactoring Process:**
1. Ensure test coverage exists
2. Make ONE small change at a time
3. Run tests after each change
4. Commit each successful step
5. Use IDE refactoring tools (Extract Method, Rename, etc.)

### 🇻🇳 Tiếng Việt

**Refactoring** là cải thiện cấu trúc code mà **không thay đổi hành vi bên ngoài**. Quan trọng: phải có test trước khi refactor!

**Các kỹ thuật phổ biến:**
1. **Extract Method**: Tách đoạn code dài thành method nhỏ có tên rõ ràng
2. **Replace Temp with Query**: Thay biến tạm bằng method call
3. **Introduce Parameter Object**: Nhóm các tham số liên quan thành object
4. **Replace Conditional with Polymorphism**: Thay `switch/if` bằng đa hình
5. **Encapsulate Field**: `public` → `private` + getter/setter
6. **Replace Magic Number**: Số `0.00087` → hằng `CONVERSION_FACTOR`

**Quy trình an toàn:**
1. Đảm bảo có tests đủ
2. Thay đổi từng bước nhỏ
3. Chạy tests sau mỗi thay đổi
4. Commit từng bước thành công

---
## Q30. What is cyclomatic complexity, and why is it important in software development?

### 🇬🇧 English

**Cyclomatic complexity** is a software metric that measures the number of independent paths through a program. It was introduced by Thomas McCabe in 1976. Higher complexity means harder to test, understand, and maintain.

**Formula:** `CC = E - N + 2P`
Where: E = edges, N = nodes, P = connected components (usually 1 for a single method)

**Simplified Rule:** Start with 1, add 1 for each: `if`, `else if`, `while`, `for`, `catch`, `&&`, `||`, `case`, `?:`

```java
// ============================================================
// Cyclomatic Complexity Examples
// ============================================================

// CC = 1 (no branches — just one path)
public double add(double a, double b) {
    return a + b;
}

// CC = 2 (one if = two paths)
public String classify(int score) {
    if (score >= 60) return "Pass";  // +1
    return "Fail";
}

// CC = 6 (complex method — should be refactored)
// Each condition adds 1: if, else if, else if, else if, &&, else if
public String getLetterGrade_BAD(int score, boolean isExtraCredit) {
    if (score < 0 || score > 100) {   // +2 (|| counts)
        return "Invalid";
    } else if (score >= 90) {          // +1
        return isExtraCredit ? "A+" : "A"; // +1 (ternary)
    } else if (score >= 80) {          // +1
        return "B";
    } else if (score >= 70) {          // +1
        return "C";
    } else {
        return "F";
    }
    // Total: 1 + 2 + 1 + 1 + 1 + 1 = 7 CC
}

// BETTER: Decompose high complexity
public String getLetterGrade(int score, boolean isExtraCredit) {
    validateScore(score);
    return determineGrade(score, isExtraCredit);
}

private void validateScore(int score) {
    if (score < 0 || score > 100) {  // CC = 2
        throw new IllegalArgumentException("Score must be 0-100, got: " + score);
    }
}

private String determineGrade(int score, boolean isExtraCredit) {  // CC = 5
    if (score >= 90) return isExtraCredit ? "A+" : "A";
    if (score >= 80) return "B";
    if (score >= 70) return "C";
    if (score >= 60) return "D";
    return "F";
}
// Each method now has lower CC — easier to test each independently

// HIGHLY COMPLEX — real-world anti-pattern
public boolean isEligibleForLoan_BAD(Customer customer, double amount, String purpose) {
    boolean eligible = false;
    if (customer != null) {
        if (customer.getCreditScore() > 700) {
            if (amount < 500_000) {
                if (customer.getAnnualIncome() > amount * 0.3) {
                    if (!purpose.equals("GAMBLING")) {
                        if (customer.getAge() >= 18 && customer.getAge() <= 70) {
                            if (customer.getEmploymentYears() >= 2) {
                                eligible = true;
                            }
                        }
                    }
                }
            }
        }
    }
    return eligible;
    // CC ≈ 9 — requires 9 test cases minimum to achieve full path coverage!
}

// BETTER: Guard clauses + decomposition
public boolean isEligibleForLoan(Customer customer, double amount, String purpose) {
    if (customer == null) return false;
    if (!hasGoodCredit(customer)) return false;
    if (!hasAdequateIncome(customer, amount)) return false;
    if (!isAcceptablePurpose(purpose)) return false;
    if (!isEligibleAge(customer)) return false;
    if (!hasSufficientEmploymentHistory(customer)) return false;
    if (amount >= 500_000) return false;
    return true;
    // CC = 7 — still improvable, but much clearer
}

private boolean hasGoodCredit(Customer c) { return c.getCreditScore() > 700; }
private boolean hasAdequateIncome(Customer c, double amount) { return c.getAnnualIncome() > amount * 0.3; }
private boolean isAcceptablePurpose(String p) { return !"GAMBLING".equals(p); }
private boolean isEligibleAge(Customer c) { return c.getAge() >= 18 && c.getAge() <= 70; }
private boolean hasSufficientEmploymentHistory(Customer c) { return c.getEmploymentYears() >= 2; }
```

**CC Guidelines:**

| CC Value | Risk | Recommendation |
|---------|------|---------------|
| 1-10 | Low | Simple, well-structured |
| 11-20 | Moderate | Consider refactoring |
| 21-50 | High | Refactoring strongly recommended |
| 50+ | Very High | Must refactor |

**Minimum test cases needed = CC** (to achieve all paths)

**Tools to measure CC:** SonarQube, PMD, Checkstyle, IDE plugins

### 🇻🇳 Tiếng Việt

**Cyclomatic Complexity (Độ phức tạp vòng)** đo số **đường đi độc lập** qua một method. Càng cao → càng khó test, khó hiểu, khó bảo trì.

**Cách tính đơn giản:** Bắt đầu từ 1, cộng thêm 1 cho mỗi: `if`, `else if`, `while`, `for`, `catch`, `&&`, `||`, `case`, `?:`

**Hướng dẫn thực tế:**
- CC 1-10: Tốt
- CC 11-20: Cân nhắc refactor
- CC > 20: Phải refactor

**Tại sao quan trọng:**
- Số test cases tối thiểu để cover đủ đường đi = CC
- Method có CC = 15 cần 15 test cases → tốn công, dễ bỏ sót
- Sau refactor mỗi method có CC ≤ 5 → dễ test, dễ hiểu

**Công cụ đo:** SonarQube, PMD, Checkstyle, IntelliJ IDEA plugin

---
## Q31. How do you enforce coding conventions in a large development team?

### 🇬🇧 English

Consistent coding conventions reduce friction, improve readability, and prevent common bugs across a large team.

**Strategy Layers:**

1. **Agree on standards** — style guides (Google Java Style, Sun Coding Conventions)
2. **Automate enforcement** — linters, formatters, static analysis
3. **Integrate into CI/CD** — fail builds for violations
4. **Code review process** — human review catches design issues

```java
// ============================================================
// Coding Convention Tools and Examples
// ============================================================

// --- Checkstyle Example (checkstyle.xml) ---
// Enforces: max line length, naming conventions, import ordering
// Run: mvn checkstyle:check

// --- PMD Example ---
// Detects: unused variables, empty catch blocks, duplicate code, CC > threshold

// --- SpotBugs (FindBugs successor) ---
// Detects: null pointer dereferences, resource leaks, synchronization issues

// --- SonarQube ---
// Comprehensive: code quality gates, technical debt tracking, security hotspots

// Example .editorconfig — cross-editor consistent formatting:
// root = true
// [*.java]
// indent_style = space
// indent_size = 4
// end_of_line = lf
// charset = utf-8
// trim_trailing_whitespace = true
// insert_final_newline = true

// ---- Examples of Convention Violations and Fixes ----

// NAMING CONVENTIONS (Java standards)
// Class names: PascalCase
class userAccount { }  // BAD — should be UserAccount
class UserAccount { }  // GOOD

// Method names: camelCase, start with verb
public int GetAge() { return 0; }  // BAD — starts with uppercase
public int getAge() { return 0; }  // GOOD

// Constants: SCREAMING_SNAKE_CASE
final double maxRetries = 3;  // BAD
static final int MAX_RETRIES = 3;  // GOOD

// Package names: lowercase, no underscores
// BAD: com.Example.MyApp
// GOOD: com.example.myapp

// ---- CODE REVIEW GUIDELINES ----
/*
 * Code Review Checklist:
 *
 * Correctness:
 * [ ] Does the code do what it's supposed to do?
 * [ ] Are edge cases handled (null, empty, overflow)?
 * [ ] Are error conditions handled properly?
 *
 * Design:
 * [ ] Does it follow SOLID principles?
 * [ ] Is there unnecessary complexity?
 * [ ] Are there code smells?
 *
 * Testing:
 * [ ] Are there unit tests for new logic?
 * [ ] Do tests cover edge cases?
 * [ ] Is test coverage adequate (>80%)?
 *
 * Performance:
 * [ ] Are there obvious performance issues (N+1 queries, O(n²))?
 * [ ] Are resources properly closed?
 *
 * Security:
 * [ ] Is input validated and sanitized?
 * [ ] Are there SQL injection / XSS risks?
 * [ ] Is sensitive data handled properly?
 */

// ---- PRE-COMMIT HOOKS (using Git hooks or Husky equivalent) ----
// In CI pipeline (GitHub Actions example):
// name: Code Quality Check
// on: [pull_request]
// jobs:
//   quality:
//     runs-on: ubuntu-latest
//     steps:
//       - uses: actions/checkout@v3
//       - uses: actions/setup-java@v3
//         with: { java-version: '17' }
//       - run: mvn checkstyle:check
//       - run: mvn pmd:check
//       - run: mvn test jacoco:report
//       - run: mvn sonar:sonar  # Optional SonarQube

// ---- FORMATTER CONFIGURATION (Google Java Format) ----
// Enforce consistent formatting automatically:
// mvn com.spotify.fmt:fmt-maven-plugin:format
// Or: google-java-format --replace **/*.java
```

**Team Enforcement Strategy:**

| Tool | Purpose | When |
|------|---------|------|
| **EditorConfig** | Basic formatting | In IDE, real-time |
| **Checkstyle** | Style conventions | Pre-commit, CI |
| **PMD** | Bug patterns, smells | CI |
| **SpotBugs** | Bug detection | CI |
| **SonarQube** | Overall quality gate | CI/CD pipeline |
| **Code Review** | Design, logic, security | PR review |

### 🇻🇳 Tiếng Việt

**Chiến lược đảm bảo coding conventions trong team:**

1. **Thống nhất tiêu chuẩn:** Chọn style guide (Google Java Style, Sun Coding Conventions)
2. **Tự động hóa:** Checkstyle, PMD, SpotBugs, SonarQube
3. **Tích hợp CI/CD:** Build fail nếu vi phạm — không ai merge code xấu
4. **Code Review:** Con người kiểm tra thiết kế, logic, bảo mật

**Quy trình khuyên dùng:**
- Developer viết code → format tự động (EditorConfig)
- Pre-commit hook → chạy Checkstyle
- CI pipeline → PMD + SpotBugs + SonarQube quality gate
- Code Review → ít nhất 1 reviewer approve

**Mẹo:** Định nghĩa "Definition of Done" bao gồm code quality metrics. Team không được phép merge nếu coverage < 80% hoặc SonarQube có critical issue.

---
## Q32. What are some common anti-patterns in software development?

### 🇬🇧 English

**Anti-patterns** are common responses to recurring problems that seem reasonable but actually make things worse. Recognizing them is the first step to avoiding them.

```java
// ============================================================
// Common Anti-Patterns with Examples
// ============================================================

// ANTI-PATTERN 1: GOD OBJECT (a.k.a. The Blob)
// One class knows and does too much
class GodObject {
    private List<User> users;
    private List<Order> orders;
    private List<Product> products;
    private Connection dbConnection;
    private EmailConfig emailConfig;
    // + 50 more fields...

    public void registerUser(String name, String email) { /* ... */ }
    public void placeOrder(String userId, List<String> items) { /* ... */ }
    public void sendEmail(String to, String subject) { /* ... */ }
    public void updateInventory(String productId, int qty) { /* ... */ }
    public void generateReport() { /* ... */ }
    // + 100 more methods...
}
// FIX: Apply SRP — split into UserService, OrderService, etc.

// ANTI-PATTERN 2: SPAGHETTI CODE — tangled, unstructured code
public void updateUserProfile_SPAGHETTI(int userId) {
    // Jumps around, hard to follow
    for (int i = 0; i < users.size(); i++) {
        if (users.get(i).getId() == userId) {
            if (users.get(i).getStatus().equals("ACTIVE")) {
                // 50 more lines of nested logic...
                if (users.get(i).getLastLogin() != null) {
                    // More nesting...
                }
            }
        }
    }
}

// ANTI-PATTERN 3: GOLDEN HAMMER
// "When you have a hammer, everything looks like a nail"
// Using one familiar solution for everything — e.g., using a relational DB
// for time-series data, or using XML for simple key-value config

// ANTI-PATTERN 4: MAGIC NUMBERS AND STRINGS
// BAD:
if (statusCode == 403) { /* ... */ }
Thread.sleep(5000);  // 5000 what? ms? Why 5000?

// GOOD:
final int HTTP_FORBIDDEN = 403;
final long RETRY_DELAY_MS = 5_000;

// ANTI-PATTERN 5: COPY-PASTE PROGRAMMING (WET Code)
// Same logic duplicated in UserController, AdminController, ApiController
// FIX: Extract to shared service/utility class

// ANTI-PATTERN 6: PREMATURE OPTIMIZATION
// Optimizing before profiling — spending time on things that don't matter
// "Premature optimization is the root of all evil" — Donald Knuth
// BAD: Manually inlining methods for speed before any performance test
// GOOD: Write clean code first, profile, then optimize hot paths

// ANTI-PATTERN 7: LAVA FLOW
// Dead code that nobody dares to remove ("it might be needed someday")
public class OrderProcessor {
    // This method has been unused since 2019, but nobody removed it
    // for fear of breaking something
    @Deprecated
    public void oldProcessOrder_LAVA(Order order) {
        System.out.println("This is never called");
    }

    // Another relic — not sure if still needed
    private static final String LEGACY_FLAG = "USE_V1_API";  // Never read
}
// FIX: Use version control confidence — if it's not used, delete it. Git has history.

// ANTI-PATTERN 8: POLTERGEIST (a.k.a. Gypsy Wagon)
// Class that does very little work and passes data to another class
class CustomerDataLoader {
    public CustomerData load(String id) {
        // All it does is call repository and return
        return customerRepository.findById(id);  // Could just call repository directly!
    }
}

// ANTI-PATTERN 9: BOAT ANCHOR
// Keeping code/hardware that is no longer used "in case it's needed"
// Old payment gateway code kept around "just in case"

// ANTI-PATTERN 10: SINGLETON OVERUSE
// Using singleton for everything, making code hard to test
public class DatabaseUtils {
    private static DatabaseUtils instance = new DatabaseUtils();
    // 50 static-accessed methods...
    // Hard to mock/test, global state everywhere
}
// FIX: Use Dependency Injection — inject dependencies instead of global singletons
```

**Anti-Pattern Summary:**

| Anti-Pattern | Problem | Fix |
|-------------|---------|-----|
| God Object | One class does everything | Apply SRP |
| Spaghetti Code | No structure, hard to follow | Refactor with clear methods |
| Magic Numbers | Unclear constants | Named constants |
| Copy-Paste | Duplicated logic | DRY, extract methods |
| Premature Optimization | Wasted effort | Profile first, then optimize |
| Lava Flow | Unused dead code | Delete with confidence |
| Singleton Overuse | Untestable global state | Dependency Injection |

### 🇻🇳 Tiếng Việt

**Anti-pattern** là các giải pháp trông có vẻ hợp lý nhưng thực ra gây hại về lâu dài.

**Các anti-pattern phổ biến:**
- **God Object**: Một class biết và làm tất cả → vi phạm SRP nghiêm trọng
- **Spaghetti Code**: Code rối rắm, không cấu trúc → khó trace, khó test
- **Magic Numbers**: `if (code == 403)` → không biết 403 là gì → dùng hằng có tên
- **Copy-Paste**: Duplicate logic ở nhiều nơi → khi fix phải sửa nhiều chỗ
- **Premature Optimization**: Tối ưu trước khi biết đâu là bottleneck → lãng phí
- **Lava Flow**: Code chết không ai dám xóa → "di tích" làm rối codebase
- **Singleton Overuse**: Global state khắp nơi → khó test, coupling cao

**Nguyên tắc:** Nhận ra anti-pattern là bước đầu tiên. Sau đó refactor dần dần, không cần rewrite toàn bộ.

---
## Q33. What is the difference between DRY and WET?

### 🇬🇧 English

**DRY (Don't Repeat Yourself):** Every piece of knowledge must have a single, unambiguous, authoritative representation in the system. Originated from "The Pragmatic Programmer" by Andy Hunt and Dave Thomas.

**WET (Write Everything Twice / We Enjoy Typing):** The opposite of DRY — same logic duplicated in multiple places.

```java
// ============================================================
// DRY vs WET Examples
// ============================================================

// ---- WET CODE: Same validation in multiple places ----
class UserService_WET {
    public void createUser(String name, String email, String password) {
        // Validation duplicated
        if (name == null || name.length() < 2 || name.length() > 50) {
            throw new IllegalArgumentException("Invalid name");
        }
        if (!email.matches("^[A-Za-z0-9+_.-]+@[A-Za-z0-9.-]+$")) {
            throw new IllegalArgumentException("Invalid email");
        }
        if (password.length() < 8 || !password.matches(".*[A-Z].*")) {
            throw new IllegalArgumentException("Weak password");
        }
        // ... create user
    }

    public void updateUser(int id, String name, String email) {
        // SAME validation repeated! (WET)
        if (name == null || name.length() < 2 || name.length() > 50) {
            throw new IllegalArgumentException("Invalid name");
        }
        if (!email.matches("^[A-Za-z0-9+_.-]+@[A-Za-z0-9.-]+$")) {
            throw new IllegalArgumentException("Invalid email");
        }
        // ... update user
    }
}
// Problem: change validation rules → must update in MULTIPLE places

// ---- DRY CODE: Single source of truth ----
// Validation logic in ONE place
public class UserValidator {
    private static final String EMAIL_REGEX = "^[A-Za-z0-9+_.-]+@[A-Za-z0-9.-]+$";
    private static final int MIN_NAME_LENGTH = 2;
    private static final int MAX_NAME_LENGTH = 50;
    private static final int MIN_PASSWORD_LENGTH = 8;

    public void validateName(String name) {
        if (name == null || name.length() < MIN_NAME_LENGTH || name.length() > MAX_NAME_LENGTH) {
            throw new IllegalArgumentException(
                String.format("Name must be %d-%d characters", MIN_NAME_LENGTH, MAX_NAME_LENGTH));
        }
    }

    public void validateEmail(String email) {
        if (email == null || !email.matches(EMAIL_REGEX)) {
            throw new IllegalArgumentException("Invalid email format: " + email);
        }
    }

    public void validatePassword(String password) {
        if (password == null || password.length() < MIN_PASSWORD_LENGTH) {
            throw new IllegalArgumentException(
                "Password must be at least " + MIN_PASSWORD_LENGTH + " characters");
        }
        if (!password.matches(".*[A-Z].*")) {
            throw new IllegalArgumentException("Password must contain at least one uppercase letter");
        }
    }
}

class UserService_DRY {
    private final UserValidator validator;

    public UserService_DRY(UserValidator validator) {
        this.validator = validator;
    }

    public void createUser(String name, String email, String password) {
        validator.validateName(name);
        validator.validateEmail(email);
        validator.validatePassword(password);
        // ... create user
    }

    public void updateUser(int id, String name, String email) {
        validator.validateName(name);
        validator.validateEmail(email);
        // ... update user
    }
}
// Change validation → update UserValidator in ONE place. Done.

// ---- DRY for Configuration ----
// WET: database config scattered in multiple files
// GOOD: single configuration source
public class AppConfig {
    public static final String DB_URL = System.getenv("DATABASE_URL");
    public static final int DB_POOL_SIZE = Integer.parseInt(
        System.getenv().getOrDefault("DB_POOL_SIZE", "10"));
    // All config in one place — change once, applies everywhere
}

// ---- BUT: Don't over-DRY (avoid wrong abstractions) ----
// Sometimes apparent duplication is actually DIFFERENT concepts
// that happen to look the same temporarily

// BAD over-abstraction: forcing unrelated things into one method
// UserReport and AuditReport look similar today but may diverge
public String generateReport_OVER_DRY(Object data, String type) {
    // Twisted abstraction to handle both cases
    if ("user".equals(type)) { /* ... */ }
    else if ("audit".equals(type)) { /* ... */ }
    // Now more complex than the original "duplication"!
}

// BETTER: Allow some duplication initially, refactor when pattern is clear
// "Duplication is far cheaper than the wrong abstraction" — Sandi Metz
public String generateUserReport(User user) { /* user-specific logic */ return ""; }
public String generateAuditReport(AuditLog audit) { /* audit-specific logic */ return ""; }
```

**DRY Principle Applied Beyond Code:**
- Database: normalize data (no redundant columns)
- Configuration: single config file/env variables
- Documentation: keep docs close to code, auto-generate from code
- Build scripts: DRY in CI/CD pipelines

**When to be careful with DRY:**
- Don't create wrong abstractions just to avoid duplication
- "The Rule of Three": refactor to DRY when same thing appears 3+ times
- Similar-looking code isn't always the same concept

### 🇻🇳 Tiếng Việt

**DRY (Don't Repeat Yourself):** Mỗi piece of knowledge chỉ có một nguồn đại diện duy nhất trong hệ thống.

**WET (Write Everything Twice):** Ngược lại — logic giống nhau bị lặp ở nhiều nơi.

**Hậu quả của WET:**
- Sửa bug → phải sửa ở nhiều chỗ → dễ bỏ sót
- Thay đổi business rule → phải tìm và sửa tất cả bản copy

**Áp dụng DRY:**
- Code: Extract method, class, utility
- Config: Central configuration file
- DB: Normalization (loại bỏ data redundancy)
- Documentation: Auto-generate từ code annotations

**Cẩn thận với "over-DRY":** "Duplication is far cheaper than the wrong abstraction" — Đừng ép tạo abstraction không tự nhiên chỉ để tránh duplicate. Khi cùng logic xuất hiện 3+ lần ("Rule of Three") mới nên extract.

---
## Q34. How do you handle exceptions properly in Java?

### 🇬🇧 English

Proper exception handling is crucial for building robust applications. Mishandled exceptions lead to poor debugging experience, data corruption, and insecure applications.

```java
// ============================================================
// Exception Handling — Best Practices
// ============================================================

// ---- CUSTOM EXCEPTION HIERARCHY ----
// Base domain exception
public class ApplicationException extends RuntimeException {
    private final String errorCode;

    public ApplicationException(String errorCode, String message) {
        super(message);
        this.errorCode = errorCode;
    }

    public ApplicationException(String errorCode, String message, Throwable cause) {
        super(message, cause);
        this.errorCode = errorCode;
    }

    public String getErrorCode() { return errorCode; }
}

public class ResourceNotFoundException extends ApplicationException {
    public ResourceNotFoundException(String resourceType, Object id) {
        super("NOT_FOUND", resourceType + " not found with id: " + id);
    }
}

public class ValidationException extends ApplicationException {
    private final Map<String, String> fieldErrors;

    public ValidationException(Map<String, String> fieldErrors) {
        super("VALIDATION_ERROR", "Validation failed: " + fieldErrors);
        this.fieldErrors = fieldErrors;
    }

    public Map<String, String> getFieldErrors() { return Collections.unmodifiableMap(fieldErrors); }
}

public class InsufficientFundsException extends ApplicationException {
    private final double available;
    private final double requested;

    public InsufficientFundsException(double available, double requested) {
        super("INSUFFICIENT_FUNDS",
            String.format("Insufficient funds: available=%.2f, requested=%.2f", available, requested));
        this.available = available;
        this.requested = requested;
    }
}

// ---- GOOD EXCEPTION HANDLING ----
public class BankService {
    private final AccountRepository accountRepository;

    public BankService(AccountRepository accountRepository) {
        this.accountRepository = accountRepository;
    }

    public void transfer(String fromId, String toId, double amount) {
        // Validate input first
        if (fromId == null) throw new IllegalArgumentException("Source account ID required");
        if (toId == null) throw new IllegalArgumentException("Target account ID required");
        if (amount <= 0) throw new IllegalArgumentException("Transfer amount must be positive");

        // Use Optional — no null checks needed
        Account from = accountRepository.findById(fromId)
            .orElseThrow(() -> new ResourceNotFoundException("Account", fromId));

        Account to = accountRepository.findById(toId)
            .orElseThrow(() -> new ResourceNotFoundException("Account", toId));

        if (from.getBalance() < amount) {
            throw new InsufficientFundsException(from.getBalance(), amount);
        }

        // Perform transfer — catch only what we can handle
        try {
            from.debit(amount);
            to.credit(amount);
            accountRepository.save(from);
            accountRepository.save(to);
        } catch (DatabaseException e) {
            // Wrap low-level exception with context
            throw new ApplicationException("TRANSFER_FAILED",
                "Transfer failed due to database error", e);
            // Never swallow exceptions silently!
        }
    }
}

// ---- COMMON ANTI-PATTERNS TO AVOID ----
public class ExceptionAntiPatterns {

    // BAD 1: Catching and ignoring exceptions (swallowing)
    public void badSwallow() {
        try {
            riskyOperation();
        } catch (Exception e) {
            // Do nothing — TERRIBLE! Hides bugs
        }
    }

    // BAD 2: Catching too broadly
    public void badTooBoard() {
        try {
            readFile();
            parseData();
            saveToDb();
        } catch (Exception e) {
            System.out.println("Something went wrong"); // Which operation? What happened?
        }
    }

    // BAD 3: Using exceptions for flow control
    public boolean isNumber_BAD(String s) {
        try {
            Integer.parseInt(s);
            return true;
        } catch (NumberFormatException e) {
            return false; // Exceptions are for EXCEPTIONAL conditions, not normal flow
        }
    }

    // GOOD: Use available methods instead
    public boolean isNumber(String s) {
        return s != null && s.matches("-?\\d+");
    }

    // BAD 4: Losing the original exception (exception chaining lost)
    public void badLostCause(String data) throws AppException {
        try {
            processData(data);
        } catch (IOException e) {
            throw new AppException("Failed"); // Original cause LOST!
        }
    }

    // GOOD: Preserve the cause
    public void goodPreserveCause(String data) throws AppException {
        try {
            processData(data);
        } catch (IOException e) {
            throw new AppException("Failed to process data", e); // Cause preserved
        }
    }

    // BAD 5: Returning null from catch blocks
    public User findUser_BAD(String id) {
        try {
            return userRepository.find(id);
        } catch (Exception e) {
            return null; // Caller gets null with no idea why
        }
    }

    // GOOD: Use Optional or rethrow with context
    public Optional<User> findUser(String id) {
        try {
            return Optional.ofNullable(userRepository.find(id));
        } catch (DatabaseException e) {
            throw new ApplicationException("DB_ERROR", "Failed to find user: " + id, e);
        }
    }

    private void riskyOperation() throws Exception {}
    private void readFile() throws IOException {}
    private void parseData() throws Exception {}
    private void saveToDb() throws Exception {}
    private void processData(String d) throws IOException {}
}

// ---- TRY-WITH-RESOURCES (Resource Management) ----
public class FileProcessor {
    public List<String> readLines(String filePath) {
        List<String> lines = new ArrayList<>();
        // Both reader and stream auto-closed — even if exception occurs
        try (var stream = Files.lines(Path.of(filePath))) {
            stream.forEach(lines::add);
        } catch (IOException e) {
            throw new ApplicationException("FILE_ERROR",
                "Failed to read file: " + filePath, e);
        }
        return lines;
    }
}
```

**Exception Handling Rules:**
1. **Throw early** — validate inputs at method entry
2. **Catch late** — let exceptions propagate to where they can be properly handled
3. **Never swallow** exceptions silently
4. **Always preserve** the original cause when re-throwing
5. **Use unchecked exceptions** for programming errors; checked for recoverable situations
6. **Create custom exceptions** for domain errors with meaningful messages
7. **Use try-with-resources** for any `Closeable`

### 🇻🇳 Tiếng Việt

**Xử lý exception đúng cách:**

**Quy tắc quan trọng:**
1. **Throw sớm, catch muộn**: Validate input ngay đầu method; để exception lan tỏa đến nơi có thể xử lý thực sự
2. **Không bao giờ bỏ qua silently**: Empty catch block là "tội ác lập trình"
3. **Preserve original cause**: Khi re-throw, luôn truyền exception gốc làm cause
4. **Custom exceptions có ý nghĩa**: `InsufficientFundsException` tốt hơn generic `Exception`
5. **Không dùng exception cho flow control**: Dùng `if` check, không dùng try-catch

**Checked vs Unchecked:**
- Checked exceptions: Tình huống có thể phục hồi (file not found, network timeout)
- Unchecked exceptions: Lỗi lập trình (null pointer, illegal argument)

**Try-with-resources**: Luôn dùng cho `Closeable` resources — tự động close dù có exception.

---
## Q35. What is the Law of Demeter, and why should it be followed?

### 🇬🇧 English

The **Law of Demeter (LoD)**, also called the **Principle of Least Knowledge**, states that an object should only communicate with its **immediate friends** — not with strangers reached through chains.

**Simple Rule:** A method should only call methods on:
1. The object itself (`this`)
2. Objects passed as parameters
3. Objects it creates locally
4. Direct fields of the class

**Not on objects obtained by calling methods of other objects (no "train wrecks").**

```java
// ============================================================
// Law of Demeter — Examples and Fixes
// ============================================================

// ---- VIOLATION: Train Wreck / Message Chain ----
// BAD: a.getB().getC().getD().doSomething()
// Each "." is another dependency — deeply coupled

public class WalletService_BAD {
    public void processPayment(Order order) {
        // Train wreck: reaching through Order → Customer → Wallet
        double balance = order.getCustomer().getWallet().getBalance();
        //                                   ^^^^^^^^^^^^^^^^^^^^^^^
        //                                   We depend on: Customer, Wallet, getBalance()
        //                                   Any change in these classes breaks us!

        if (balance >= order.getTotal()) {
            order.getCustomer().getWallet().debit(order.getTotal());
            System.out.println("Payment of $" + order.getTotal() + " processed");
        }
    }

    // ANOTHER VIOLATION:
    public String getCustomerCity(Order order) {
        return order.getCustomer().getAddress().getCity().toUpperCase();
        // Breaks if: getCustomer() returns null, getAddress() returns null,
        // or any of these structures change
    }
}

// ---- COMPLIANT DESIGN ----
// Each class is responsible for exposing what others need

public class Wallet {
    private double balance;

    public boolean hasSufficientFunds(double amount) {
        return balance >= amount;
    }

    public boolean debit(double amount) {
        if (!hasSufficientFunds(amount)) return false;
        balance -= amount;
        return true;
    }

    public double getBalance() { return balance; }

    public void credit(double amount) { balance += amount; }
}

public class Customer {
    private String name;
    private Wallet wallet;
    private Address address;

    // Customer delegates to Wallet — hides the detail from outsiders
    public boolean canAfford(double amount) {
        return wallet.hasSufficientFunds(amount);
    }

    public boolean processPayment(double amount) {
        return wallet.debit(amount);
    }

    // Customer exposes city directly — no need to go through Address
    public String getCity() {
        return address != null ? address.getCity() : "Unknown";
    }

    public String getName() { return name; }
}

public class Order {
    private Customer customer;
    private List<OrderLineItem> items;

    public double getTotal() {
        return items.stream().mapToDouble(i -> i.price() * i.quantity()).sum();
    }

    // Order delegates payment to Customer — hides wallet chain
    public boolean canBePaid() {
        return customer.canAfford(getTotal());
    }

    public boolean pay() {
        return customer.processPayment(getTotal());
    }

    public String getCustomerCity() {
        return customer.getCity();  // One dot — Law of Demeter compliant
    }
}

public class WalletService_GOOD {
    public void processPayment(Order order) {
        // Clean: Order handles its own payment logic
        if (order.canBePaid()) {
            boolean success = order.pay();
            if (success) {
                System.out.println("Payment processed for order: " + order.getTotal());
            }
        } else {
            throw new InsufficientFundsException(0, order.getTotal()); // simplified
        }
    }
}
```

**Benefits of following Law of Demeter:**
- Reduced coupling — changes to `Wallet` don't ripple through every class that touches `Order`
- Easier to test — each class can be tested with simple mocks
- Better encapsulation — internal structures are hidden
- Better readability — no confusing chain calls

**Real-World Analogy:** You ask your friend to ask their contact to find information for you. You don't need to meet the contact directly — your friend delegates.

### 🇻🇳 Tiếng Việt

**Luật Demeter (Law of Demeter):** Một phương thức chỉ nên gọi phương thức trên **đối tượng quen biết trực tiếp** — không phải đối tượng được lấy qua chuỗi gọi.

**Vi phạm — "Train Wreck":** `order.getCustomer().getWallet().getBalance()` — 3 dấu chấm, phụ thuộc vào Customer, Wallet, và getBalance — bất kỳ thay đổi nào đều có thể phá vỡ code.

**Cách fix:** Mỗi class cung cấp phương thức "delegate" che đi sự phức tạp bên trong:
- `Customer.canAfford(amount)` thay vì `customer.getWallet().hasSufficientFunds(amount)`
- `Order.pay()` thay vì `order.getCustomer().getWallet().debit(...)`

**Lợi ích:** Giảm coupling, dễ test, dễ thay đổi cấu trúc nội bộ mà không ảnh hưởng code bên ngoài.

---
## Q36. What is test-driven development (TDD), and how does it improve code quality?

### 🇬🇧 English

**TDD (Test-Driven Development)** is a development practice where you write failing tests BEFORE writing production code, then write minimal code to make tests pass, then refactor.

**The Red-Green-Refactor Cycle:**
1. 🔴 **Red** — Write a failing test (it should fail because code doesn't exist yet)
2. 🟢 **Green** — Write minimal code to make the test pass
3. 🔵 **Refactor** — Clean up code while keeping tests green

```java
// ============================================================
// TDD Example — Building a ShoppingCart from scratch
// ============================================================

// STEP 1: Write failing test (RED)
import org.junit.jupiter.api.*;
import static org.junit.jupiter.api.Assertions.*;

class ShoppingCartTest {

    private ShoppingCart cart;

    @BeforeEach
    void setUp() {
        cart = new ShoppingCart();  // Class doesn't exist yet — compile error
    }

    // Test 1: New cart is empty
    @Test
    @DisplayName("New cart should have zero items and zero total")
    void newCartIsEmpty() {
        assertEquals(0, cart.getItemCount());
        assertEquals(0.0, cart.getTotal(), 0.001);
    }

    // Test 2: Add item increases count
    @Test
    @DisplayName("Adding item increases item count")
    void addItemIncreasesCount() {
        cart.addItem("Laptop", 999.99, 1);
        assertEquals(1, cart.getItemCount());
    }

    // Test 3: Total is calculated correctly
    @Test
    @DisplayName("Total reflects added items")
    void totalCalculatedCorrectly() {
        cart.addItem("Laptop", 999.99, 1);
        cart.addItem("Mouse", 29.99, 2);
        double expectedTotal = 999.99 + (29.99 * 2); // 1059.97
        assertEquals(expectedTotal, cart.getTotal(), 0.001);
    }

    // Test 4: Remove item
    @Test
    @DisplayName("Removing item decreases count")
    void removeItemDecreasesCount() {
        cart.addItem("Laptop", 999.99, 1);
        cart.addItem("Mouse", 29.99, 2);
        cart.removeItem("Mouse");
        assertEquals(1, cart.getItemCount());
        assertEquals(999.99, cart.getTotal(), 0.001);
    }

    // Test 5: Discount application
    @Test
    @DisplayName("10% discount reduces total correctly")
    void applyDiscountReducesTotal() {
        cart.addItem("Laptop", 1000.0, 1);
        cart.applyDiscount(10.0);  // 10%
        assertEquals(900.0, cart.getTotal(), 0.001);
    }

    // Test 6: Quantity validation
    @Test
    @DisplayName("Adding negative quantity throws exception")
    void negativeQuantityThrowsException() {
        assertThrows(IllegalArgumentException.class,
            () -> cart.addItem("Laptop", 999.99, -1));
    }

    // Test 7: Clear cart
    @Test
    @DisplayName("Clear cart removes all items")
    void clearCartEmptiesEverything() {
        cart.addItem("Laptop", 999.99, 1);
        cart.addItem("Mouse", 29.99, 2);
        cart.clear();
        assertEquals(0, cart.getItemCount());
        assertEquals(0.0, cart.getTotal(), 0.001);
    }
}

// STEP 2: Write minimal implementation (GREEN)
public class ShoppingCart {
    private final Map<String, CartItem> items = new HashMap<>();
    private double discountPercent = 0;

    public void addItem(String name, double price, int quantity) {
        if (quantity <= 0) {
            throw new IllegalArgumentException("Quantity must be positive, got: " + quantity);
        }
        if (price < 0) {
            throw new IllegalArgumentException("Price cannot be negative");
        }
        items.merge(name,
            new CartItem(name, price, quantity),
            (existing, newItem) -> new CartItem(name, price, existing.quantity() + quantity));
    }

    public void removeItem(String name) {
        items.remove(name);
    }

    public int getItemCount() {
        return items.values().stream().mapToInt(CartItem::quantity).sum();
    }

    public double getTotal() {
        double subtotal = items.values().stream()
            .mapToDouble(item -> item.price() * item.quantity())
            .sum();
        return subtotal * (1 - discountPercent / 100);
    }

    public void applyDiscount(double discountPercent) {
        if (discountPercent < 0 || discountPercent > 100) {
            throw new IllegalArgumentException("Discount must be 0-100%");
        }
        this.discountPercent = discountPercent;
    }

    public void clear() {
        items.clear();
        discountPercent = 0;
    }

    public List<CartItem> getItems() {
        return Collections.unmodifiableList(new ArrayList<>(items.values()));
    }

    // STEP 3: Refactor — extract CartItem record, improve method names, etc.
    public record CartItem(String name, double price, int quantity) {
        public double subtotal() { return price * quantity; }
    }
}

// Additional benefit: tests serve as living documentation
// Anyone reading tests understands the expected behavior
```

**Benefits of TDD:**
- Drives better design — hard-to-test code signals design problems
- 100% coverage of new code (every line written to make a test pass)
- Regression safety — tests catch when changes break things
- Living documentation — tests show how code is supposed to behave
- Reduces debugging — errors are caught immediately

**TDD vs Traditional Testing:**

| Aspect | TDD | Traditional |
|--------|-----|-------------|
| When tests written | Before code | After code |
| Coverage | Near 100% | Often <60% |
| Design feedback | Immediate | Late |
| Debugging | Minimal | Extensive |

### 🇻🇳 Tiếng Việt

**TDD (Test-Driven Development)** là phương pháp viết **test trước, code sau**. Vòng lặp: Red → Green → Refactor.

**Chu trình:**
1. 🔴 **Red**: Viết test cho tính năng chưa có → test fail
2. 🟢 **Green**: Viết code tối thiểu để test pass
3. 🔵 **Refactor**: Cải thiện code, test vẫn phải pass

**Lợi ích:**
- Buộc thiết kế tốt hơn: code khó test → code cần refactor
- Coverage cao: mọi dòng code đều được test
- Safety net: refactor tự tin vì test bắt regression
- Documentation sống: test mô tả behavior mong đợi

**Ví dụ:** Trước khi viết `ShoppingCart.addItem()`, viết test `addItemIncreasesCount()` → test fail (class chưa có) → viết `ShoppingCart` → test pass → refactor.

**TDD không phải lúc nào cũng khả thi:** UI code, legacy code, prototypes — nhưng cho business logic thì rất hiệu quả.

---
## Q37. How do you use logging effectively in a Java application?

### 🇬🇧 English

Effective logging provides visibility into application behavior without exposing sensitive data or degrading performance.

```java
// ============================================================
// Logging Best Practices in Java (SLF4J + Logback)
// ============================================================

import org.slf4j.Logger;
import org.slf4j.LoggerFactory;

public class OrderService {
    // Use SLF4J facade — not tied to specific logging implementation
    private static final Logger logger = LoggerFactory.getLogger(OrderService.class);

    private final OrderRepository orderRepository;
    private final PaymentGateway paymentGateway;

    public OrderService(OrderRepository orderRepository, PaymentGateway paymentGateway) {
        this.orderRepository = orderRepository;
        this.paymentGateway = paymentGateway;
    }

    public Order placeOrder(String customerId, List<OrderLineItem> items) {
        // DEBUG: Detailed tracing (only enabled in development)
        logger.debug("Placing order for customer: {}, items: {}", customerId, items.size());

        Order order = new Order(customerId, items);

        // INFO: Business events (always logged)
        logger.info("Order created: orderId={}, customerId={}, total={}",
            order.getOrderId(), customerId, order.getTotal());

        try {
            PaymentResult payment = paymentGateway.charge(customerId, order.getTotal(), "USD");

            if (payment.success()) {
                order.setStatus(OrderStatus.CONFIRMED);
                orderRepository.save(order);
                logger.info("Order confirmed: orderId={}, transactionId={}",
                    order.getOrderId(), payment.transactionId());
            } else {
                logger.warn("Payment declined: orderId={}, reason={}",
                    order.getOrderId(), payment.message());
                order.setStatus(OrderStatus.CANCELLED);
            }

        } catch (PaymentGatewayException e) {
            // ERROR: System failures requiring attention
            logger.error("Payment gateway error for order: orderId={}, customerId={}",
                order.getOrderId(), customerId, e);  // Exception as last arg — includes stack trace
            throw new ApplicationException("PAYMENT_ERROR", "Payment processing failed", e);
        } catch (Exception e) {
            // Log unexpected exceptions with full context
            logger.error("Unexpected error placing order: orderId={}", order.getOrderId(), e);
            throw new ApplicationException("ORDER_ERROR", "Failed to place order", e);
        }

        return order;
    }

    // SENSITIVE DATA — never log passwords, credit card numbers, tokens
    public void authenticateUser(String username, String password) {
        logger.info("Authentication attempt: username={}", username);
        // NEVER: logger.info("Auth: username={}, password={}", username, password);

        // MDC (Mapped Diagnostic Context) — add context to all log messages
        org.slf4j.MDC.put("userId", username);
        try {
            // ... authentication logic ...
            logger.info("Authentication successful: username={}", username);
        } finally {
            org.slf4j.MDC.clear();  // Always clear MDC
        }
    }

    // Performance logging
    public List<Order> searchOrders(String customerId, String status) {
        long startTime = System.currentTimeMillis();
        logger.debug("Searching orders: customerId={}, status={}", customerId, status);

        List<Order> results = orderRepository.findByCustomerAndStatus(customerId, status);

        long duration = System.currentTimeMillis() - startTime;
        if (duration > 1000) {  // Log slow queries as warning
            logger.warn("Slow order search: duration={}ms, customerId={}, resultCount={}",
                duration, customerId, results.size());
        } else {
            logger.debug("Order search completed: duration={}ms, resultCount={}",
                duration, results.size());
        }

        return results;
    }
}

// Logback configuration (logback.xml):
/*
<configuration>
    <appender name="CONSOLE" class="ch.qos.logback.core.ConsoleAppender">
        <encoder>
            <pattern>%d{HH:mm:ss.SSS} [%thread] %-5level %logger{36} - %msg%n</pattern>
        </encoder>
    </appender>

    <appender name="FILE" class="ch.qos.logback.core.rolling.RollingFileAppender">
        <file>logs/application.log</file>
        <rollingPolicy class="ch.qos.logback.core.rolling.TimeBasedRollingPolicy">
            <fileNamePattern>logs/application.%d{yyyy-MM-dd}.%i.log</fileNamePattern>
            <maxFileSize>100MB</maxFileSize>
            <maxHistory>30</maxHistory>
        </rollingPolicy>
        <encoder>
            <pattern>%d{ISO8601} [%thread] %-5level [%X{userId}] %logger{36} - %msg%n</pattern>
        </encoder>
    </appender>

    <root level="INFO">
        <appender-ref ref="CONSOLE" />
        <appender-ref ref="FILE" />
    </root>

    <logger name="com.example" level="DEBUG" />
</configuration>
*/
```

**Log Levels:**
| Level | Use For |
|-------|---------|
| `TRACE` | Very detailed flow (rarely used in prod) |
| `DEBUG` | Debugging info (disabled in prod) |
| `INFO` | Business events, milestones |
| `WARN` | Recoverable problems, degraded behavior |
| `ERROR` | Failures requiring attention |

**Rules:**
- Use SLF4J (not `System.out.println` or `java.util.logging`)
- Use parameterized logging: `logger.info("user={}", user)` not string concat
- Never log sensitive data (passwords, tokens, PII)
- Log enough context to diagnose issues without restarting
- Use MDC for correlation IDs in distributed systems

### 🇻🇳 Tiếng Việt

**Logging hiệu quả:** Cung cấp visibility vào ứng dụng mà không ảnh hưởng hiệu năng hay lộ dữ liệu nhạy cảm.

**Nguyên tắc:**
1. Dùng **SLF4J** (facade) + Logback/Log4j2 (implementation) — linh hoạt thay thế
2. Dùng **parameterized logging**: `logger.info("user={}", user)` — không concat string khi log
3. **KHÔNG bao giờ log** mật khẩu, token, số thẻ tín dụng, dữ liệu cá nhân
4. Log đủ context để diagnosis mà không cần deploy lại

**Log levels:**
- `DEBUG`: Chi tiết, chỉ bật khi debug
- `INFO`: Sự kiện business quan trọng (order placed, user logged in)
- `WARN`: Vấn đề không nghiêm trọng (slow query, retry)
- `ERROR`: Lỗi cần xử lý (payment failed, DB error)

**MDC (Mapped Diagnostic Context):** Gắn context (userId, requestId) vào tất cả log messages trong thread — rất hữu ích trong distributed systems.

---
## Q38. What is the benefit of writing self-documenting code?

### 🇬🇧 English

**Self-documenting code** communicates its intent so clearly through naming and structure that comments are unnecessary for understanding *what* it does. Comments should explain *why*, not *what*.

```java
// ============================================================
// Self-Documenting Code — Before and After
// ============================================================

// ---- BEFORE: Cryptic, needs comments ----
public boolean chk(User u, int d, double a) {
    // Check if user is eligible for withdrawal
    if (u.tp == 1 && u.b >= a && (System.currentTimeMillis()/1000 - u.la) < d*86400) {
        u.b -= a;
        return true;
    }
    return false;
}

// ---- AFTER: Self-documenting ----
public boolean processWithdrawal(User user, int sessionTimeoutDays, double withdrawalAmount) {
    boolean isAccountActive = user.getAccountType() == AccountType.PREMIUM;
    boolean hasSufficientBalance = user.getBalance() >= withdrawalAmount;
    boolean isSessionValid = isWithinSessionTimeout(user.getLastActivityTimestamp(), sessionTimeoutDays);

    if (!isAccountActive || !hasSufficientBalance || !isSessionValid) {
        return false;
    }

    user.debit(withdrawalAmount);
    return true;
}

private boolean isWithinSessionTimeout(long lastActivityEpochSeconds, int timeoutDays) {
    long currentEpochSeconds = System.currentTimeMillis() / 1000;
    long timeoutSeconds = (long) timeoutDays * 24 * 60 * 60;
    return (currentEpochSeconds - lastActivityEpochSeconds) < timeoutSeconds;
}

// ---- More Examples of Self-Documenting Practices ----

// 1. EXPRESSIVE BOOLEAN VARIABLES
// BAD:
if (employee.type != 0 && employee.months / 12 > 5) { }

// GOOD:
boolean isFullTimeEmployee = employee.getType() == EmployeeType.FULL_TIME;
boolean hasMoreThanFiveYearsTenure = employee.getMonthsOfService() / 12 > 5;
boolean isEligibleForSabbatical = isFullTimeEmployee && hasMoreThanFiveYearsTenure;
if (isEligibleForSabbatical) { }

// 2. DESCRIPTIVE METHOD NAMES (verb + noun)
// BAD: process(), handle(), doStuff(), update()
// GOOD:
void sendPasswordResetEmail(User user) { }
boolean isOlderThan(int ageInYears) { return false; }
List<Order> findPendingOrdersOlderThan(Duration duration) { return null; }
void calculateMonthlyInterestAndUpdateBalance() { }

// 3. POSITIVE CONDITIONS
// BAD: hard to parse double negatives
if (!isNotAuthenticated) { }

// GOOD:
if (isAuthenticated) { }
if (!isEmpty()) { }

// 4. NAMED RETURN VALUES
// BAD:
return user != null && user.getAge() >= 18 && user.getCountry().equals("US")
    && !user.isBanned() && user.getEmailVerified();

// GOOD:
boolean userExists = user != null;
boolean isAdult = user != null && user.getAge() >= 18;
boolean isUsResident = user != null && "US".equals(user.getCountry());
boolean isGoodStanding = user != null && !user.isBanned() && user.getEmailVerified();
return userExists && isAdult && isUsResident && isGoodStanding;

// 5. AVOIDING COMMENTS THAT LIE (outdated comments)
// Code changes, comments don't — leads to misinformation
// BAD:
// Returns the sum of x and y
public int multiply(int x, int y) { return x * y; }  // Comment is WRONG after refactor!

// GOOD: Code speaks for itself
public int multiply(int x, int y) { return x * y; }

// 6. WHEN COMMENTS ARE VALUABLE (explain WHY)
// This sorting order is intentional — the UI depends on stable order
// See: https://jira.example.com/PROJ-1234
Collections.sort(items, Comparator.comparing(Item::getId));

// MD5 is intentional here — legacy API requires MD5, not security
String legacyHash = md5(apiKey + timestamp);

// Skip the first result — it's always a header row from the external API
for (int i = 1; i < results.size(); i++) { }
```

**Benefits of self-documenting code:**
- No stale comments (comments can lie; code cannot)
- Faster code reviews — no need to cross-reference comments and code
- Onboarding is faster — new developers understand code without documentation
- Forces clearer thinking — if you can't name it well, the design may be unclear

### 🇻🇳 Tiếng Việt

**Self-documenting code (Code tự tài liệu hóa):** Code được viết rõ ràng đến mức không cần comment để giải thích *nó làm gì* — tên biến, method, class đã nói lên tất cả.

**Lợi ích:**
- Comment không bao giờ lỗi thời — code là nguồn sự thật
- Review code nhanh hơn
- Onboard developer mới dễ hơn
- Buộc phải suy nghĩ rõ ràng về thiết kế

**Kỹ thuật:**
1. **Tên biến mô tả:** `isEligibleForSabbatical` thay vì `flag`
2. **Tên method rõ ràng:** `findPendingOrdersOlderThan(duration)` thay vì `getOrders()`
3. **Điều kiện Boolean có tên:** Extract điều kiện phức tạp thành biến có tên
4. **Tránh double negative:** `if (isAuthenticated)` thay vì `if (!isNotAuthenticated)`

**Khi nào dùng comment:** Giải thích **TẠI SAO** (lý do thiết kế, business decision, workaround cho bug thư viện), không giải thích **LÀM GÌ** (code đã nói điều đó).

---
## Q39. How do you implement dependency injection in Java?

### 🇬🇧 English

**Dependency Injection (DI)** is a design pattern where objects receive their dependencies from outside rather than creating them internally. It's the practical implementation of the Dependency Inversion Principle.

**Three Types of DI:**
1. **Constructor injection** — dependencies passed via constructor (recommended)
2. **Setter injection** — dependencies set via setters (optional dependencies)
3. **Field injection** — dependencies injected into fields (framework-specific, avoid in non-Spring)

```java
// ============================================================
// Dependency Injection — Manual and Spring
// ============================================================

// ---- INTERFACES (Abstractions) ----
public interface UserRepository {
    Optional<User> findById(String id);
    User save(User user);
    boolean existsByEmail(String email);
}

public interface PasswordEncoder {
    String encode(String rawPassword);
    boolean matches(String rawPassword, String encodedPassword);
}

public interface EventPublisher {
    void publish(Object event);
}

// ---- MANUAL DEPENDENCY INJECTION ----
// No framework — pure Java
public class UserService {
    private final UserRepository userRepository;     // Interface dependency
    private final PasswordEncoder passwordEncoder;   // Interface dependency
    private final EventPublisher eventPublisher;     // Interface dependency

    // CONSTRUCTOR INJECTION — all dependencies required
    // Makes dependencies explicit and testable
    public UserService(UserRepository userRepository,
                       PasswordEncoder passwordEncoder,
                       EventPublisher eventPublisher) {
        this.userRepository = Objects.requireNonNull(userRepository, "UserRepository required");
        this.passwordEncoder = Objects.requireNonNull(passwordEncoder, "PasswordEncoder required");
        this.eventPublisher = Objects.requireNonNull(eventPublisher, "EventPublisher required");
    }

    public User registerUser(String name, String email, String rawPassword) {
        if (userRepository.existsByEmail(email)) {
            throw new ValidationException(Map.of("email", "Email already in use"));
        }

        User user = new User(name, email, passwordEncoder.encode(rawPassword));
        User saved = userRepository.save(user);
        eventPublisher.publish(new UserRegisteredEvent(saved));
        return saved;
    }

    public boolean authenticate(String email, String rawPassword) {
        return userRepository.findById(email)
            .map(user -> passwordEncoder.matches(rawPassword, user.getPasswordHash()))
            .orElse(false);
    }
}

// ---- IMPLEMENTATIONS ----
public class BCryptPasswordEncoder implements PasswordEncoder {
    private static final int ROUNDS = 12;

    @Override
    public String encode(String rawPassword) {
        // Real implementation: BCrypt.hashpw(rawPassword, BCrypt.gensalt(ROUNDS))
        return "bcrypt:" + rawPassword.hashCode();
    }

    @Override
    public boolean matches(String rawPassword, String encodedPassword) {
        return encodedPassword.equals(encode(rawPassword));
    }
}

public class InMemoryUserRepository implements UserRepository {
    private final Map<String, User> store = new HashMap<>();

    @Override
    public Optional<User> findById(String id) { return Optional.ofNullable(store.get(id)); }

    @Override
    public User save(User user) { store.put(user.getId(), user); return user; }

    @Override
    public boolean existsByEmail(String email) {
        return store.values().stream().anyMatch(u -> email.equals(u.getEmail()));
    }
}

public class LoggingEventPublisher implements EventPublisher {
    private static final Logger logger = LoggerFactory.getLogger(LoggingEventPublisher.class);

    @Override
    public void publish(Object event) {
        logger.info("Event published: {}", event);
    }
}

// ---- COMPOSITION ROOT — Wire everything up ----
// In a real app, this is your main class or Spring configuration
public class ApplicationConfig {
    public static UserService createUserService() {
        UserRepository repository = new InMemoryUserRepository();
        PasswordEncoder encoder = new BCryptPasswordEncoder();
        EventPublisher publisher = new LoggingEventPublisher();
        return new UserService(repository, encoder, publisher);
    }
}

// ---- SPRING FRAMEWORK DI (using annotations) ----
// Spring automatically detects and injects dependencies
/*
@Service
public class UserServiceSpring {
    private final UserRepository userRepository;
    private final PasswordEncoder passwordEncoder;
    private final ApplicationEventPublisher eventPublisher;

    // Spring auto-injects constructor parameters
    @Autowired  // Optional if only one constructor
    public UserServiceSpring(UserRepository userRepository,
                              PasswordEncoder passwordEncoder,
                              ApplicationEventPublisher eventPublisher) {
        this.userRepository = userRepository;
        this.passwordEncoder = passwordEncoder;
        this.eventPublisher = eventPublisher;
    }
}

@Repository
public class JpaUserRepository implements UserRepository { ... }

@Configuration
public class SecurityConfig {
    @Bean
    public PasswordEncoder passwordEncoder() {
        return new BCryptPasswordEncoder(12);
    }
}
*/

// ---- TESTING: The real benefit of DI ----
class UserServiceTest {
    @Test
    void registerUser_withDuplicateEmail_throwsValidationException() {
        // Inject test doubles — no real database, no real email service
        UserRepository mockRepo = new InMemoryUserRepository();
        PasswordEncoder mockEncoder = (password) -> "hashed_" + password;
        EventPublisher noOpPublisher = event -> {};  // No-op for testing

        UserService service = new UserService(mockRepo,
            new PasswordEncoder() {
                public String encode(String p) { return "hashed"; }
                public boolean matches(String raw, String enc) { return enc.equals("hashed"); }
            },
            noOpPublisher);

        service.registerUser("Alice", "alice@test.com", "Password1!");

        // Try to register again with same email
        assertThrows(ValidationException.class,
            () -> service.registerUser("Alice2", "alice@test.com", "Password2!"));
    }
}
```

**DI Benefits:**
- Testability — inject mocks instead of real implementations
- Flexibility — swap implementations without changing business logic
- Clarity — dependencies are explicit, not hidden
- Single responsibility — class doesn't manage its own dependencies

### 🇻🇳 Tiếng Việt

**Dependency Injection (DI):** Thay vì class tự tạo dependencies (`new MySQLRepo()`), dependencies được **truyền vào từ bên ngoài**.

**3 cách inject:**
1. **Constructor Injection** (khuyến nghị): Dependencies bắt buộc, rõ ràng, immutable
2. **Setter Injection**: Dependencies tùy chọn, có thể thay sau khởi tạo
3. **Field Injection** (tránh dùng ngoài Spring): Ẩn dependency, khó test

**Lợi ích:**
- **Testability**: Trong unit test, inject mock thay vì real DB, real email service
- **Flexibility**: Đổi implementation → chỉ thay class inject vào, không sửa business logic
- **Clarity**: Dependencies hiện rõ trong constructor signature

**Spring DI:** Spring tự động detect (`@Service`, `@Repository`) và inject. `@Autowired` trên constructor (optional nếu chỉ có 1 constructor).

---
## Q40. What are some best practices for designing modular and reusable code?

### 🇬🇧 English

Modular, reusable code reduces duplication, speeds up development, and makes the system easier to reason about.

```java
// ============================================================
// Modular and Reusable Code Practices
// ============================================================

// PRACTICE 1: Design to interfaces, not implementations
// Makes modules interchangeable and independently testable
public interface Sortable<T extends Comparable<T>> {
    void sort(List<T> items);
}

public class QuickSort<T extends Comparable<T>> implements Sortable<T> {
    @Override
    public void sort(List<T> items) {
        if (items.size() <= 1) return;
        quicksort(items, 0, items.size() - 1);
    }
    private void quicksort(List<T> items, int low, int high) { /* ... */ }
}

public class MergeSort<T extends Comparable<T>> implements Sortable<T> {
    @Override
    public void sort(List<T> items) { /* merge sort implementation */ }
}

// Can swap sorting algorithms without changing clients
public class DataProcessor<T extends Comparable<T>> {
    private Sortable<T> sorter;  // Depends on interface
    public DataProcessor(Sortable<T> sorter) { this.sorter = sorter; }
    public List<T> process(List<T> data) {
        sorter.sort(data);
        return data;
    }
}

// PRACTICE 2: Utility classes — static methods for pure functions
public final class StringUtils {
    private StringUtils() { }  // Prevent instantiation

    public static String capitalize(String input) {
        if (input == null || input.isEmpty()) return input;
        return Character.toUpperCase(input.charAt(0)) + input.substring(1).toLowerCase();
    }

    public static String truncate(String input, int maxLength, String suffix) {
        if (input == null || input.length() <= maxLength) return input;
        return input.substring(0, maxLength - suffix.length()) + suffix;
    }

    public static boolean isNullOrBlank(String input) {
        return input == null || input.isBlank();
    }
}

// PRACTICE 3: Generic utility methods
public final class CollectionUtils {
    private CollectionUtils() {}

    public static <T> List<List<T>> partition(List<T> list, int batchSize) {
        List<List<T>> partitions = new ArrayList<>();
        for (int i = 0; i < list.size(); i += batchSize) {
            partitions.add(new ArrayList<>(
                list.subList(i, Math.min(i + batchSize, list.size()))
            ));
        }
        return partitions;
    }

    public static <T> Optional<T> findFirst(List<T> list, java.util.function.Predicate<T> predicate) {
        return list.stream().filter(predicate).findFirst();
    }

    public static <T, R> List<R> mapList(List<T> list, java.util.function.Function<T, R> mapper) {
        return list.stream().map(mapper).collect(java.util.stream.Collectors.toList());
    }
}

// PRACTICE 4: Builder pattern for flexible object construction
public class QueryBuilder {
    private String table;
    private List<String> columns = new ArrayList<>();
    private List<String> conditions = new ArrayList<>();
    private String orderBy;
    private Integer limit;
    private Integer offset;

    public QueryBuilder from(String table) {
        this.table = table;
        return this;
    }

    public QueryBuilder select(String... cols) {
        columns.addAll(Arrays.asList(cols));
        return this;
    }

    public QueryBuilder where(String condition) {
        conditions.add(condition);
        return this;
    }

    public QueryBuilder orderBy(String column) {
        this.orderBy = column;
        return this;
    }

    public QueryBuilder limit(int limit) {
        this.limit = limit;
        return this;
    }

    public QueryBuilder offset(int offset) {
        this.offset = offset;
        return this;
    }

    public String build() {
        StringBuilder sql = new StringBuilder("SELECT ");
        sql.append(columns.isEmpty() ? "*" : String.join(", ", columns));
        sql.append(" FROM ").append(table);
        if (!conditions.isEmpty()) {
            sql.append(" WHERE ").append(String.join(" AND ", conditions));
        }
        if (orderBy != null) sql.append(" ORDER BY ").append(orderBy);
        if (limit != null) sql.append(" LIMIT ").append(limit);
        if (offset != null) sql.append(" OFFSET ").append(offset);
        return sql.toString();
    }
}

// Usage — fluent, readable, reusable
String query = new QueryBuilder()
    .from("orders")
    .select("id", "customer_id", "total")
    .where("status = 'PENDING'")
    .where("total > 100")
    .orderBy("created_at DESC")
    .limit(20)
    .offset(0)
    .build();
// SELECT id, customer_id, total FROM orders WHERE status = 'PENDING' AND total > 100 ORDER BY created_at DESC LIMIT 20 OFFSET 0

// PRACTICE 5: Package by feature (not by layer)
// BAD: com.example.controllers, com.example.services, com.example.repositories
// GOOD: com.example.orders, com.example.users, com.example.products
// Feature packages keep related code together, support team autonomy
```

**Best Practices Summary:**
1. **Design to interfaces** — swap implementations freely
2. **Small, focused classes** — single responsibility, easier to reuse
3. **Pure functions** for utilities — no side effects, easily testable
4. **Generics** for type-safe reusable components
5. **Package by feature** — cohesive modules
6. **Builder pattern** for complex object construction
7. **Avoid static state** in reusable components

### 🇻🇳 Tiếng Việt

**Thiết kế module hóa và tái sử dụng:**

1. **Design to interfaces**: Phụ thuộc vào abstraction → dễ thay thế implementation
2. **Utility classes tĩnh**: Các pure function không có side effects → dễ tái sử dụng và test
3. **Generics**: Viết code một lần, dùng cho nhiều kiểu dữ liệu
4. **Builder pattern**: Xây dựng object phức tạp theo cách flexible, readable
5. **Package by feature**: Nhóm code theo tính năng (orders, users) thay vì layer (controllers, services) — cohesion cao hơn

**Dấu hiệu module hóa tốt:**
- Module A có thể hoạt động độc lập, test độc lập
- Thay đổi trong module A không ảnh hưởng module B trừ khi có dependency rõ ràng
- Code có thể được import và dùng trong project khác mà không cần thay đổi

---
# 🎨 PART 3: Design Patterns

---
## Q41. What are design patterns, and why are they useful?

### 🇬🇧 English

**Design patterns** are proven, reusable solutions to commonly occurring problems in software design. They were popularized by the "Gang of Four" (GoF) book: *Design Patterns: Elements of Reusable Object-Oriented Software* by Erich Gamma, Richard Helm, Ralph Johnson, and John Vlissides (1994).

**Three Categories of Design Patterns:**

| Category | Purpose | Examples |
|----------|---------|---------|
| **Creational** | How objects are created | Singleton, Factory, Builder, Prototype, Abstract Factory |
| **Structural** | How objects are composed | Adapter, Bridge, Decorator, Facade, Proxy, Composite |
| **Behavioral** | How objects communicate | Observer, Strategy, Command, Iterator, Template Method, Chain of Responsibility |

```java
// ============================================================
// Design Patterns Overview
// ============================================================

// CREATIONAL: Factory Method — create objects without specifying exact class
interface Logger {
    void log(String message);
    LogLevel getLevel();
}

enum LogLevel { DEBUG, INFO, WARNING, ERROR }

class ConsoleLogger implements Logger {
    private final LogLevel level;
    public ConsoleLogger(LogLevel level) { this.level = level; }
    @Override public void log(String message) {
        System.out.println("[CONSOLE][" + level + "] " + message);
    }
    @Override public LogLevel getLevel() { return level; }
}

class FileLogger implements Logger {
    private final String filePath;
    private final LogLevel level;
    public FileLogger(String filePath, LogLevel level) {
        this.filePath = filePath;
        this.level = level;
    }
    @Override public void log(String message) {
        System.out.println("[FILE:" + filePath + "][" + level + "] " + message);
    }
    @Override public LogLevel getLevel() { return level; }
}

// Factory — creates appropriate Logger based on config
class LoggerFactory2 {
    public static Logger createLogger(String type, String config, LogLevel level) {
        return switch (type.toUpperCase()) {
            case "CONSOLE" -> new ConsoleLogger(level);
            case "FILE" -> new FileLogger(config, level);
            default -> throw new IllegalArgumentException("Unknown logger type: " + type);
        };
    }
}

// STRUCTURAL: Decorator — add behavior without changing class
interface TextProcessor {
    String process(String text);
}

class PlainTextProcessor implements TextProcessor {
    @Override public String process(String text) { return text; }
}

class UpperCaseDecorator implements TextProcessor {
    private final TextProcessor wrapped;
    public UpperCaseDecorator(TextProcessor wrapped) { this.wrapped = wrapped; }
    @Override public String process(String text) { return wrapped.process(text).toUpperCase(); }
}

class TrimDecorator implements TextProcessor {
    private final TextProcessor wrapped;
    public TrimDecorator(TextProcessor wrapped) { this.wrapped = wrapped; }
    @Override public String process(String text) { return wrapped.process(text).trim(); }
}

class StarWrapDecorator implements TextProcessor {
    private final TextProcessor wrapped;
    public StarWrapDecorator(TextProcessor wrapped) { this.wrapped = wrapped; }
    @Override public String process(String text) { return "*** " + wrapped.process(text) + " ***"; }
}

// BEHAVIORAL: Command — encapsulate operations as objects
interface Command {
    void execute();
    void undo();
}

class TextEditor {
    private StringBuilder content = new StringBuilder();
    private Deque<Command> history = new ArrayDeque<>();

    public void executeCommand(Command command) {
        command.execute();
        history.push(command);
    }

    public void undoLast() {
        if (!history.isEmpty()) {
            history.pop().undo();
        }
    }

    public void append(String text) { content.append(text); }
    public void delete(int from, int to) { content.delete(from, to); }
    public String getContent() { return content.toString(); }
}

public class DesignPatternOverview {
    public static void main(String[] args) {
        // Creational: Factory
        Logger logger = LoggerFactory2.createLogger("CONSOLE", null, LogLevel.INFO);
        logger.log("Application started");

        // Structural: Decorator — chain processors
        TextProcessor processor = new StarWrapDecorator(
            new UpperCaseDecorator(
                new TrimDecorator(
                    new PlainTextProcessor())));
        System.out.println(processor.process("  hello world  "));
        // Output: *** HELLO WORLD ***

        // Behavioral: Observer (simplified)
        System.out.println("Design patterns overview complete.");
    }
}
```

**Why Design Patterns are Useful:**
- ✅ Proven solutions — battle-tested over decades
- ✅ Common vocabulary — "use Observer pattern" communicates instantly
- ✅ Avoid reinventing the wheel
- ✅ Documentation and maintainability — team understands structure
- ✅ Extensibility — patterns are designed to be extended

**Caution:** Don't over-engineer. Use patterns when they solve a real problem, not just to use them.

### 🇻🇳 Tiếng Việt

**Design Patterns (Mẫu thiết kế)** là các giải pháp tái sử dụng đã được kiểm chứng cho các vấn đề phổ biến trong thiết kế phần mềm.

**3 nhóm chính:**
- **Creational (Khởi tạo)**: Cách tạo object — Singleton, Factory, Builder
- **Structural (Cấu trúc)**: Cách kết hợp objects — Adapter, Decorator, Facade
- **Behavioral (Hành vi)**: Cách objects tương tác — Observer, Strategy, Command

**Tại sao hữu ích:**
- Giải pháp đã được kiểm chứng — không cần phát minh lại
- Ngôn ngữ chung: "dùng Observer" — developer khác hiểu ngay
- Hỗ trợ extensibility và maintainability

**Cảnh báo:** Không dùng pattern chỉ để dùng. Design patterns giải quyết vấn đề cụ thể — overengineering là anti-pattern!

---
## Q42. Explain the Factory pattern and provide an example.

### 🇬🇧 English

The **Factory pattern** is a creational pattern that provides an interface for creating objects, allowing subclasses or methods to decide which concrete class to instantiate. This decouples object creation from usage.

**Variants:**
- **Simple Factory**: A static method creates objects (not a formal GoF pattern)
- **Factory Method**: Defines an interface for creating an object, subclasses decide the class
- **Abstract Factory**: Creates families of related objects

```java
// ============================================================
// Factory Pattern — Notification System
// ============================================================

// PRODUCT interface
public interface Notification {
    void send(String recipient, String title, String message);
    String getType();
    boolean supports(String channel);
}

// CONCRETE PRODUCTS
public class EmailNotification implements Notification {
    private final String smtpHost;
    private final int smtpPort;

    public EmailNotification(String smtpHost, int smtpPort) {
        this.smtpHost = smtpHost;
        this.smtpPort = smtpPort;
    }

    @Override
    public void send(String recipient, String title, String message) {
        System.out.printf("[EMAIL via %s:%d] To: %s | Subject: %s | Body: %s%n",
            smtpHost, smtpPort, recipient, title, message);
        // Real: javax.mail or Spring JavaMailSender
    }

    @Override public String getType() { return "EMAIL"; }
    @Override public boolean supports(String channel) { return "email".equalsIgnoreCase(channel); }
}

public class SmsNotification implements Notification {
    private final String apiKey;
    private final String senderNumber;

    public SmsNotification(String apiKey, String senderNumber) {
        this.apiKey = apiKey;
        this.senderNumber = senderNumber;
    }

    @Override
    public void send(String recipient, String title, String message) {
        System.out.printf("[SMS from %s] To: %s | Message: %s%n",
            senderNumber, recipient, message);
        // Real: Twilio API, AWS SNS, etc.
    }

    @Override public String getType() { return "SMS"; }
    @Override public boolean supports(String channel) { return "sms".equalsIgnoreCase(channel); }
}

public class PushNotification implements Notification {
    private final String fcmApiKey;

    public PushNotification(String fcmApiKey) { this.fcmApiKey = fcmApiKey; }

    @Override
    public void send(String recipient, String title, String message) {
        System.out.printf("[PUSH via FCM] DeviceToken: %s | Title: %s | Body: %s%n",
            recipient, title, message);
        // Real: Firebase Cloud Messaging, APNs
    }

    @Override public String getType() { return "PUSH"; }
    @Override public boolean supports(String channel) {
        return "push".equalsIgnoreCase(channel) || "fcm".equalsIgnoreCase(channel);
    }
}

public class SlackNotification implements Notification {
    private final String webhookUrl;

    public SlackNotification(String webhookUrl) { this.webhookUrl = webhookUrl; }

    @Override
    public void send(String recipient, String title, String message) {
        System.out.printf("[SLACK] Channel: %s | %s: %s%n", recipient, title, message);
    }

    @Override public String getType() { return "SLACK"; }
    @Override public boolean supports(String channel) { return "slack".equalsIgnoreCase(channel); }
}

// FACTORY METHOD PATTERN
// Base creator — defines the factory method
public abstract class NotificationFactory {
    // FACTORY METHOD — subclasses decide which concrete class to create
    public abstract Notification createNotification();

    // Template method — uses the factory method
    public void sendNotification(String recipient, String title, String message) {
        Notification notification = createNotification();
        System.out.println("Sending " + notification.getType() + " notification...");
        notification.send(recipient, title, message);
    }
}

// Concrete creator 1
public class EmailNotificationFactory extends NotificationFactory {
    private final String smtpHost;
    private final int smtpPort;

    public EmailNotificationFactory(String smtpHost, int smtpPort) {
        this.smtpHost = smtpHost;
        this.smtpPort = smtpPort;
    }

    @Override
    public Notification createNotification() {
        return new EmailNotification(smtpHost, smtpPort);
    }
}

// Concrete creator 2
public class SmsNotificationFactory extends NotificationFactory {
    @Override
    public Notification createNotification() {
        return new SmsNotification("twilio-api-key", "+1-800-NOTIFY");
    }
}

// SIMPLE FACTORY — registry-based (practical approach)
public class NotificationRegistry {
    private final Map<String, Notification> registry = new HashMap<>();

    public NotificationRegistry() {
        // Register available notification types
        registry.put("email", new EmailNotification("smtp.example.com", 587));
        registry.put("sms", new SmsNotification("sms-api-key", "+15551234567"));
        registry.put("push", new PushNotification("fcm-server-key"));
        registry.put("slack", new SlackNotification("https://hooks.slack.com/..."));
    }

    public Notification getNotification(String channel) {
        Notification n = registry.get(channel.toLowerCase());
        if (n == null) throw new IllegalArgumentException("Unsupported channel: " + channel);
        return n;
    }

    public void sendNotification(String channel, String recipient, String title, String message) {
        getNotification(channel).send(recipient, title, message);
    }
}

// ABSTRACT FACTORY — creates families of related objects
// Use case: different themes (Light/Dark) with matching Button + Checkbox + Dialog
public interface Button { void render(); void onClick(); }
public interface Checkbox { void render(); boolean isChecked(); }

public class LightButton implements Button {
    @Override public void render() { System.out.println("[Light Button] rendered in white"); }
    @Override public void onClick() { System.out.println("[Light Button] clicked"); }
}

public class DarkButton implements Button {
    @Override public void render() { System.out.println("[Dark Button] rendered in dark"); }
    @Override public void onClick() { System.out.println("[Dark Button] clicked"); }
}

public class LightCheckbox implements Checkbox {
    private boolean checked;
    @Override public void render() { System.out.println("[Light Checkbox] " + (checked ? "☑" : "☐")); }
    @Override public boolean isChecked() { return checked; }
}

public class DarkCheckbox implements Checkbox {
    private boolean checked;
    @Override public void render() { System.out.println("[Dark Checkbox] " + (checked ? "☑" : "☐")); }
    @Override public boolean isChecked() { return checked; }
}

// Abstract Factory — creates matching UI components
public interface UIFactory {
    Button createButton();
    Checkbox createCheckbox();
}

public class LightThemeFactory implements UIFactory {
    @Override public Button createButton() { return new LightButton(); }
    @Override public Checkbox createCheckbox() { return new LightCheckbox(); }
}

public class DarkThemeFactory implements UIFactory {
    @Override public Button createButton() { return new DarkButton(); }
    @Override public Checkbox createCheckbox() { return new DarkCheckbox(); }
}

// Application doesn't know which theme — just uses the factory
public class Application {
    private final UIFactory uiFactory;

    public Application(UIFactory uiFactory) { this.uiFactory = uiFactory; }

    public void render() {
        Button btn = uiFactory.createButton();  // Could be Light or Dark
        Checkbox chk = uiFactory.createCheckbox();
        btn.render();
        chk.render();
        btn.onClick();
    }
}

public class FactoryPatternDemo {
    public static void main(String[] args) {
        // Factory Method
        NotificationFactory emailFactory = new EmailNotificationFactory("smtp.example.com", 587);
        emailFactory.sendNotification("user@example.com", "Welcome!", "Hello there!");

        NotificationFactory smsFactory = new SmsNotificationFactory();
        smsFactory.sendNotification("+15551234567", "Alert", "Your code is 123456");

        // Simple Factory (registry)
        NotificationRegistry registry = new NotificationRegistry();
        registry.sendNotification("slack", "#alerts", "System Alert", "Server CPU > 90%");
        registry.sendNotification("push", "device-token-xyz", "New Message", "You have mail!");

        // Abstract Factory
        System.out.println("\n--- Light Theme ---");
        new Application(new LightThemeFactory()).render();

        System.out.println("\n--- Dark Theme ---");
        new Application(new DarkThemeFactory()).render();
    }
}
```

**When to Use Factory Pattern:**
- When object creation involves complex logic
- When you want to decouple creation from usage
- When the exact class to create depends on runtime conditions
- When you want to centralize object creation for consistency

### 🇻🇳 Tiếng Việt

**Factory Pattern** cung cấp interface để tạo objects, che giấu logic khởi tạo phức tạp và tách biệt việc tạo object khỏi việc sử dụng.

**3 biến thể:**
1. **Simple Factory**: Static method tạo object dựa trên tham số
2. **Factory Method**: Lớp cha định nghĩa template, lớp con quyết định tạo object nào
3. **Abstract Factory**: Tạo *họ* các objects liên quan (Button + Checkbox + Dialog theo theme)

**Ví dụ thực tế:**
- `NotificationRegistry`: Tạo `EmailNotification`, `SmsNotification`, `PushNotification` dựa trên channel string
- `UIFactory`: Tạo bộ UI components theo Light/Dark theme
- JDBC `DriverManager.getConnection()`: Factory cho database connections

**Khi nào dùng:**
- Logic khởi tạo phức tạp
- Loại object phụ thuộc vào runtime conditions
- Muốn tập trung logic tạo object

---
## Q43. How does the Singleton pattern work, and what are its pros and cons?

### 🇬🇧 English

*See also Q18 for implementation details.*

The **Singleton** pattern ensures only **one instance** of a class exists and provides a global access point.

```java
// ============================================================
// Singleton — Production-Grade Implementation + Testing
// ============================================================

// Thread-safe Singleton using Initialization-on-demand Holder (recommended)
public class CacheManager {
    // Configuration
    private final int maxEntries;
    private final long expiryMs;

    // Thread-safe cache
    private final Map<String, CacheEntry> cache =
        new java.util.concurrent.ConcurrentHashMap<>();

    private CacheManager() {
        this.maxEntries = 1000;
        this.expiryMs = 3600 * 1000L; // 1 hour
        System.out.println("CacheManager initialized");
    }

    private static class Holder {
        private static final CacheManager INSTANCE = new CacheManager();
    }

    public static CacheManager getInstance() {
        return Holder.INSTANCE;
    }

    public void put(String key, Object value) {
        if (cache.size() >= maxEntries) {
            evictOldest();
        }
        cache.put(key, new CacheEntry(value, System.currentTimeMillis()));
    }

    public Optional<Object> get(String key) {
        CacheEntry entry = cache.get(key);
        if (entry == null) return Optional.empty();
        if (System.currentTimeMillis() - entry.createdAt() > expiryMs) {
            cache.remove(key);
            return Optional.empty();
        }
        return Optional.of(entry.value());
    }

    public void invalidate(String key) {
        cache.remove(key);
    }

    public void clear() {
        cache.clear();
    }

    public int size() {
        return cache.size();
    }

    private void evictOldest() {
        // Simple eviction: remove entries that are expired
        long now = System.currentTimeMillis();
        cache.entrySet().removeIf(e -> now - e.getValue().createdAt() > expiryMs);
    }

    private record CacheEntry(Object value, long createdAt) {}
}

// Using CacheManager
public class UserService2 {
    private static final CacheManager cache = CacheManager.getInstance();

    public User getUser(String userId) {
        return (User) cache.get("user:" + userId).orElseGet(() -> {
            User user = loadFromDatabase(userId);
            cache.put("user:" + userId, user);
            return user;
        });
    }

    private User loadFromDatabase(String id) {
        System.out.println("Loading user from DB: " + id);
        return new User(); // Simulated
    }
}

// Singleton for Configuration Management
public enum ConfigurationManager {
    INSTANCE;

    private final Properties properties = new Properties();

    {
        // Load configuration on instantiation
        try {
            properties.load(getClass().getClassLoader()
                .getResourceAsStream("application.properties"));
        } catch (Exception e) {
            System.err.println("Failed to load properties, using defaults");
        }
        // Set defaults
        properties.putIfAbsent("server.port", "8080");
        properties.putIfAbsent("db.pool.size", "10");
    }

    public String get(String key) {
        return properties.getProperty(key);
    }

    public String get(String key, String defaultValue) {
        return properties.getProperty(key, defaultValue);
    }

    public int getInt(String key, int defaultValue) {
        String value = properties.getProperty(key);
        if (value == null) return defaultValue;
        try { return Integer.parseInt(value); }
        catch (NumberFormatException e) { return defaultValue; }
    }
}
```

**Pros of Singleton:**
- ✅ Controlled access to single resource (config, logger, connection pool)
- ✅ Saves memory — only one instance
- ✅ Lazy initialization possible (Bill Pugh idiom)
- ✅ Thread-safe when implemented correctly

**Cons of Singleton:**
- ❌ Global state — difficult to test (can't reset between tests)
- ❌ Tight coupling — hard to swap implementation
- ❌ Hides dependencies — makes code harder to understand
- ❌ Not easily replaceable with mock in unit tests
- ❌ Multi-classloader issues in complex environments

**Modern Alternative:** Use Dependency Injection (Spring `@Bean` with default singleton scope):
```java
@Configuration
public class AppConfig {
    @Bean  // Singleton by default in Spring
    public CacheManager cacheManager() {
        return new CacheManager();
    }
}

@Service
public class UserService3 {
    private final CacheManager cache;  // Injected, not global
    public UserService3(CacheManager cache) { this.cache = cache; }
    // Can be tested by injecting a mock CacheManager!
}
```

### 🇻🇳 Tiếng Việt

*(Xem thêm Q18 cho chi tiết implementation)*

**Ưu điểm Singleton:**
- Kiểm soát truy cập vào resource dùng chung (config, logger, pool)
- Tiết kiệm bộ nhớ — chỉ một instance

**Nhược điểm:**
- Global state → khó test (không reset được giữa các test)
- Coupling chặt → khó thay thế bằng mock
- Ẩn dependencies

**Giải pháp hiện đại:** Dùng Spring DI với `@Bean` singleton scope thay vì tự implement Singleton. Spring quản lý lifecycle, dễ test với mock injection.

---
## Q44. What is the difference between the Adapter and Bridge design patterns?

### 🇬🇧 English

Both patterns deal with abstraction and implementation, but for different purposes:

| Aspect | Adapter | Bridge |
|--------|---------|--------|
| **Intent** | Make incompatible interfaces work together | Decouple abstraction from implementation |
| **When** | After the fact (retrofit) | Upfront design |
| **Problem** | "I need to use this class but it has the wrong interface" | "I need to vary both abstraction and implementation independently" |
| **Analogy** | Power plug adapter (convert existing) | Remote control + device (design-time separation) |

```java
// ============================================================
// ADAPTER PATTERN
// ============================================================

// EXISTING legacy service (third-party, cannot modify)
class LegacyPaymentGateway {
    public String makePayment(int amount, String currency, String cardNumber) {
        return "LEGACY_TXN_" + System.currentTimeMillis();
    }

    public boolean reversePayment(String transactionCode) {
        return true;
    }
}

// NEW interface our application expects
interface ModernPaymentProcessor {
    PaymentResult processPayment(PaymentRequest request);
    boolean refundPayment(String transactionId, double amount);
}

// ADAPTER: Makes LegacyPaymentGateway conform to ModernPaymentProcessor
// Wraps the legacy class and translates calls
class LegacyPaymentAdapter implements ModernPaymentProcessor {
    private final LegacyPaymentGateway legacy;

    public LegacyPaymentAdapter(LegacyPaymentGateway legacy) {
        this.legacy = legacy;
    }

    @Override
    public PaymentResult processPayment(PaymentRequest request) {
        // ADAPT: Convert from ModernPaymentProcessor's format to legacy format
        int amountInCents = (int)(request.amount() * 100);
        String cardNumber = request.metadata().getOrDefault("cardNumber", "UNKNOWN");

        String transactionCode = legacy.makePayment(amountInCents, request.currency(), cardNumber);

        return new PaymentResult(true, transactionCode, "Payment processed via legacy gateway");
    }

    @Override
    public boolean refundPayment(String transactionId, double amount) {
        return legacy.reversePayment(transactionId);
    }
}

// Client uses ModernPaymentProcessor — doesn't know about legacy
class CheckoutService {
    private final ModernPaymentProcessor processor;

    public CheckoutService(ModernPaymentProcessor processor) {
        this.processor = processor;
    }

    public void checkout(String orderId, double amount, String currency) {
        PaymentRequest request = new PaymentRequest(orderId, amount, currency, new HashMap<>());
        PaymentResult result = processor.processPayment(request);
        System.out.println("Checkout result: " + result.message());
    }
}

// ============================================================
// BRIDGE PATTERN
// ============================================================

// The key idea: TWO DIMENSIONS of variation, both extensible independently
// Dimension 1: Type of Shape (Circle, Rectangle, Triangle...)
// Dimension 2: Rendering method (Vector, Raster, SVG...)

// IMPLEMENTOR interface (Rendering)
interface Renderer {
    void renderCircle(double x, double y, double radius);
    void renderRectangle(double x, double y, double width, double height);
    String getRendererType();
}

// Concrete Implementors
class VectorRenderer implements Renderer {
    @Override
    public void renderCircle(double x, double y, double radius) {
        System.out.printf("[Vector] Drawing circle at (%.0f,%.0f) radius=%.0f%n", x, y, radius);
    }

    @Override
    public void renderRectangle(double x, double y, double width, double height) {
        System.out.printf("[Vector] Drawing rect at (%.0f,%.0f) size=%.0fx%.0f%n", x, y, width, height);
    }

    @Override
    public String getRendererType() { return "Vector"; }
}

class RasterRenderer implements Renderer {
    @Override
    public void renderCircle(double x, double y, double radius) {
        System.out.printf("[Raster] Drawing %d pixels for circle at (%.0f,%.0f)%n",
            (int)(Math.PI * radius * radius), x, y);
    }

    @Override
    public void renderRectangle(double x, double y, double width, double height) {
        System.out.printf("[Raster] Drawing %d pixels for rect at (%.0f,%.0f)%n",
            (int)(width * height), x, y);
    }

    @Override
    public String getRendererType() { return "Raster"; }
}

// ABSTRACTION class (Shape)
// Contains reference to Renderer — this IS the bridge
abstract class Shape2 {
    protected final Renderer renderer;  // Bridge to implementation
    protected double x, y;

    protected Shape2(Renderer renderer, double x, double y) {
        this.renderer = renderer;
        this.x = x;
        this.y = y;
    }

    public abstract void draw();
    public abstract void resize(double factor);
    public String getInfo() {
        return getClass().getSimpleName() + " using " + renderer.getRendererType() + " renderer";
    }
}

// Refined Abstractions — vary independently of renderer
class Circle2 extends Shape2 {
    private double radius;

    public Circle2(Renderer renderer, double x, double y, double radius) {
        super(renderer, x, y);
        this.radius = radius;
    }

    @Override
    public void draw() {
        renderer.renderCircle(x, y, radius);
    }

    @Override
    public void resize(double factor) {
        radius *= factor;
    }
}

class Rectangle2 extends Shape2 {
    private double width, height;

    public Rectangle2(Renderer renderer, double x, double y, double width, double height) {
        super(renderer, x, y);
        this.width = width;
        this.height = height;
    }

    @Override
    public void draw() {
        renderer.renderRectangle(x, y, width, height);
    }

    @Override
    public void resize(double factor) {
        width *= factor;
        height *= factor;
    }
}

public class AdapterBridgeDemo {
    public static void main(String[] args) {
        // ADAPTER: Integrating legacy system
        LegacyPaymentGateway legacy = new LegacyPaymentGateway();
        ModernPaymentProcessor modernized = new LegacyPaymentAdapter(legacy);
        CheckoutService checkout = new CheckoutService(modernized);
        checkout.checkout("ORD-001", 99.99, "USD");

        // BRIDGE: Mix shapes with renderers freely
        Renderer vector = new VectorRenderer();
        Renderer raster = new RasterRenderer();

        Shape2[] shapes = {
            new Circle2(vector, 10, 10, 5),      // Circle + Vector
            new Circle2(raster, 20, 20, 8),      // Circle + Raster
            new Rectangle2(vector, 0, 0, 10, 5), // Rectangle + Vector
            new Rectangle2(raster, 5, 5, 7, 3)  // Rectangle + Raster
        };

        for (Shape2 shape : shapes) {
            System.out.println(shape.getInfo());
            shape.draw();
        }
        // Can add new shapes (Triangle) or new renderers (SVG) independently!
    }
}
```

**Key Difference in One Sentence:**
- **Adapter**: "I have an existing incompatible interface — adapt it." (Retrofit)
- **Bridge**: "I'm designing this from scratch — let abstraction and implementation evolve separately." (Design-time)

### 🇻🇳 Tiếng Việt

**Adapter Pattern:**
- **Mục đích**: Làm hai interface không tương thích hoạt động cùng nhau
- **Thời điểm**: Khi tích hợp thư viện/service bên ngoài có interface khác
- **Ví dụ**: Adapter ổ điện (biến 220V → 110V)

**Bridge Pattern:**
- **Mục đích**: Tách abstraction khỏi implementation để cả hai có thể thay đổi độc lập
- **Thời điểm**: Thiết kế ngay từ đầu khi có 2 chiều biến thiên độc lập
- **Ví dụ**: Remote control (abstraction) + TV/Radio/AC (implementation) — bất kỳ remote nào có thể điều khiển bất kỳ thiết bị nào

**Cách nhớ:** Adapter = "fix" problem, Bridge = "prevent" problem.

---
## Q45. How does the Observer pattern work, and where is it commonly used?

### 🇬🇧 English

The **Observer pattern** (also called Publish-Subscribe or Event pattern) defines a one-to-many dependency between objects. When one object (Subject/Publisher) changes state, all its dependents (Observers/Subscribers) are notified automatically.

```java
// ============================================================
// Observer Pattern — Stock Market Event System
// ============================================================

// OBSERVER INTERFACE
public interface StockObserver {
    void onPriceChanged(String symbol, double oldPrice, double newPrice);
}

// SUBJECT INTERFACE
public interface StockMarket {
    void subscribe(String symbol, StockObserver observer);
    void unsubscribe(String symbol, StockObserver observer);
    void setPrice(String symbol, double price);
}

// CONCRETE SUBJECT — holds state and notifies observers
public class StockExchange implements StockMarket {
    // Map from stock symbol to current price
    private final Map<String, Double> stockPrices = new HashMap<>();
    // Map from stock symbol to list of observers
    private final Map<String, List<StockObserver>> observerMap = new HashMap<>();

    @Override
    public void subscribe(String symbol, StockObserver observer) {
        observerMap.computeIfAbsent(symbol, k -> new ArrayList<>()).add(observer);
        System.out.println("Subscribed to " + symbol + ": " + observer.getClass().getSimpleName());
    }

    @Override
    public void unsubscribe(String symbol, StockObserver observer) {
        List<StockObserver> observers = observerMap.get(symbol);
        if (observers != null) {
            observers.remove(observer);
            System.out.println("Unsubscribed from " + symbol);
        }
    }

    @Override
    public void setPrice(String symbol, double newPrice) {
        double oldPrice = stockPrices.getOrDefault(symbol, 0.0);
        stockPrices.put(symbol, newPrice);

        if (oldPrice != newPrice) {
            notifyObservers(symbol, oldPrice, newPrice);
        }
    }

    private void notifyObservers(String symbol, double oldPrice, double newPrice) {
        List<StockObserver> observers = observerMap.getOrDefault(symbol, Collections.emptyList());
        // Notify all subscribers for this symbol
        for (StockObserver observer : new ArrayList<>(observers)) { // Copy to avoid ConcurrentModification
            observer.onPriceChanged(symbol, oldPrice, newPrice);
        }
    }

    public double getPrice(String symbol) {
        return stockPrices.getOrDefault(symbol, 0.0);
    }
}

// CONCRETE OBSERVERS
// Observer 1: Trading bot that auto-buys on price drop
public class AutoTrader implements StockObserver {
    private final String traderId;
    private final double buyThresholdPercent;  // Buy if drops by this %
    private double portfolio = 100_000.0;  // Starting cash
    private final Map<String, Integer> holdings = new HashMap<>();

    public AutoTrader(String traderId, double buyThresholdPercent) {
        this.traderId = traderId;
        this.buyThresholdPercent = buyThresholdPercent;
    }

    @Override
    public void onPriceChanged(String symbol, double oldPrice, double newPrice) {
        if (oldPrice == 0) return;

        double changePercent = (newPrice - oldPrice) / oldPrice * 100;

        if (changePercent <= -buyThresholdPercent && portfolio >= newPrice) {
            // Price dropped enough — buy!
            int shares = (int)(portfolio * 0.1 / newPrice);  // Buy with 10% of portfolio
            if (shares > 0) {
                portfolio -= shares * newPrice;
                holdings.merge(symbol, shares, Integer::sum);
                System.out.printf("[%s] BOUGHT %d shares of %s at $%.2f " +
                    "(drop: %.1f%%) Portfolio: $%.2f%n",
                    traderId, shares, symbol, newPrice, changePercent, portfolio);
            }
        }
    }

    public Map<String, Integer> getHoldings() { return Collections.unmodifiableMap(holdings); }
}

// Observer 2: Alert service that notifies users via email/SMS
public class PriceAlertService implements StockObserver {
    private final Map<String, Double> alertThresholds = new HashMap<>();

    public void setAlert(String symbol, double targetPrice) {
        alertThresholds.put(symbol, targetPrice);
        System.out.println("Alert set: " + symbol + " @ $" + targetPrice);
    }

    @Override
    public void onPriceChanged(String symbol, double oldPrice, double newPrice) {
        Double threshold = alertThresholds.get(symbol);
        if (threshold == null) return;

        boolean crossedAbove = oldPrice < threshold && newPrice >= threshold;
        boolean crossedBelow = oldPrice > threshold && newPrice <= threshold;

        if (crossedAbove) {
            System.out.printf("[ALERT] %s crossed ABOVE $%.2f! Current: $%.2f%n",
                symbol, threshold, newPrice);
            sendNotification(symbol, "ABOVE", threshold, newPrice);
        } else if (crossedBelow) {
            System.out.printf("[ALERT] %s crossed BELOW $%.2f! Current: $%.2f%n",
                symbol, threshold, newPrice);
            sendNotification(symbol, "BELOW", threshold, newPrice);
        }
    }

    private void sendNotification(String symbol, String direction, double threshold, double price) {
        // In real app: send email, SMS, push notification
        System.out.printf("[NOTIFY] User: %s price went %s target $%.2f (actual: $%.2f)%n",
            symbol, direction, threshold, price);
    }
}

// Observer 3: Analytics/Dashboard
public class MarketDashboard implements StockObserver {
    private final Map<String, List<Double>> priceHistory = new HashMap<>();

    @Override
    public void onPriceChanged(String symbol, double oldPrice, double newPrice) {
        priceHistory.computeIfAbsent(symbol, k -> new ArrayList<>()).add(newPrice);
        double change = newPrice - oldPrice;
        double changePct = oldPrice > 0 ? (change / oldPrice * 100) : 0;
        String arrow = change >= 0 ? "▲" : "▼";
        System.out.printf("[DASHBOARD] %s: $%.2f %s %.2f (%.2f%%)%n",
            symbol, newPrice, arrow, Math.abs(change), Math.abs(changePct));
    }

    public double getAveragePrice(String symbol) {
        List<Double> history = priceHistory.getOrDefault(symbol, Collections.emptyList());
        return history.stream().mapToDouble(Double::doubleValue).average().orElse(0);
    }
}

// JAVA BUILT-IN OBSERVER (using functional approach with lambdas)
// Modern Java approach using java.util.function
public class EventBus<T> {
    private final List<java.util.function.Consumer<T>> listeners = new ArrayList<>();

    public void subscribe(java.util.function.Consumer<T> listener) {
        listeners.add(listener);
    }

    public void unsubscribe(java.util.function.Consumer<T> listener) {
        listeners.remove(listener);
    }

    public void publish(T event) {
        listeners.forEach(listener -> listener.accept(event));
    }
}

public class ObserverPatternDemo {
    public static void main(String[] args) {
        StockExchange exchange = new StockExchange();

        // Create observers
        AutoTrader bot = new AutoTrader("Bot-Alpha", 5.0); // Buy if drops 5%
        PriceAlertService alertService = new PriceAlertService();
        MarketDashboard dashboard = new MarketDashboard();

        // Set up alerts
        alertService.setAlert("AAPL", 150.0);
        alertService.setAlert("GOOGL", 2800.0);

        // Subscribe to specific stocks
        exchange.subscribe("AAPL", dashboard);
        exchange.subscribe("AAPL", alertService);
        exchange.subscribe("AAPL", bot);
        exchange.subscribe("GOOGL", dashboard);
        exchange.subscribe("GOOGL", alertService);

        // Simulate market activity
        System.out.println("\n=== Market Opens ===");
        exchange.setPrice("AAPL", 155.0);
        exchange.setPrice("GOOGL", 2750.0);

        System.out.println("\n=== Price Changes ===");
        exchange.setPrice("AAPL", 148.0);   // Drop — alert triggered, bot might buy
        exchange.setPrice("AAPL", 152.0);   // Rise — alert triggered again
        exchange.setPrice("GOOGL", 2810.0); // GOOGL crosses above alert threshold

        System.out.println("\n=== Unsubscribe bot from AAPL ===");
        exchange.unsubscribe("AAPL", bot);
        exchange.setPrice("AAPL", 140.0);  // Bot won't respond

        System.out.println("\nAAPL avg: $" + String.format("%.2f", dashboard.getAveragePrice("AAPL")));

        // Modern lambda-based EventBus
        System.out.println("\n=== Lambda EventBus ===");
        EventBus<String> eventBus = new EventBus<>();
        eventBus.subscribe(event -> System.out.println("Listener 1: " + event));
        eventBus.subscribe(event -> System.out.println("Listener 2 (uppercase): " + event.toUpperCase()));
        eventBus.publish("order placed");
    }
}
```

**Where Observer Pattern is Used:**
- **Java AWT/Swing**: `ActionListener`, `MouseListener`
- **Spring Framework**: `ApplicationEventPublisher`, `@EventListener`
- **RxJava/Project Reactor**: Reactive streams (Observables, Flux)
- **Android**: `LiveData`, `Flow`
- **GUI frameworks**: Button click handlers
- **Message queues**: Kafka consumers, RabbitMQ subscribers
- **Model-View-Controller (MVC)**: View observes Model

### 🇻🇳 Tiếng Việt

**Observer Pattern** (còn gọi Publish-Subscribe): Định nghĩa quan hệ 1-nhiều — khi Subject thay đổi trạng thái, tất cả Observers được thông báo tự động.

**Thành phần:**
- **Subject (Publisher)**: Giữ danh sách observers, notify khi state thay đổi
- **Observer (Subscriber)**: Interface với method `update()`/`onEvent()`
- **Concrete Observer**: Xử lý notification theo cách riêng

**Ứng dụng thực tế:**
- GUI: Button listener, event handlers
- Spring: `@EventListener`, `ApplicationEventPublisher`
- Stock ticker, cryptocurrency price feeds
- Social media notifications (new post → notify followers)
- Kafka/RabbitMQ consumers

**Lưu ý:** 
- Tránh memory leak: luôn `unsubscribe` khi observer không còn cần
- Thread safety: notify trong môi trường concurrent cần synchronized

---
## Q46. What is the Strategy pattern, and how does it help with code flexibility?

### 🇬🇧 English

The **Strategy pattern** defines a family of algorithms, encapsulates each one, and makes them interchangeable. It lets the algorithm vary independently from clients that use it.

This is one of the most commonly used patterns and is the behavioral counterpart to the Open/Closed Principle.

```java
// ============================================================
// Strategy Pattern — Multiple Real-World Examples
// ============================================================

// ============== EXAMPLE 1: Sorting Strategy ==============
public interface SortStrategy<T extends Comparable<T>> {
    void sort(List<T> data);
    String name();
    String bestCase();
}

public class BubbleSortStrategy<T extends Comparable<T>> implements SortStrategy<T> {
    @Override
    public void sort(List<T> data) {
        int n = data.size();
        for (int i = 0; i < n - 1; i++) {
            for (int j = 0; j < n - i - 1; j++) {
                if (data.get(j).compareTo(data.get(j + 1)) > 0) {
                    T temp = data.get(j);
                    data.set(j, data.get(j + 1));
                    data.set(j + 1, temp);
                }
            }
        }
    }
    @Override public String name() { return "Bubble Sort"; }
    @Override public String bestCase() { return "O(n²)"; }
}

public class QuickSortStrategy<T extends Comparable<T>> implements SortStrategy<T> {
    @Override
    public void sort(List<T> data) {
        quickSort(data, 0, data.size() - 1);
    }

    private void quickSort(List<T> data, int low, int high) {
        if (low < high) {
            int pivot = partition(data, low, high);
            quickSort(data, low, pivot - 1);
            quickSort(data, pivot + 1, high);
        }
    }

    private int partition(List<T> data, int low, int high) {
        T pivot = data.get(high);
        int i = low - 1;
        for (int j = low; j < high; j++) {
            if (data.get(j).compareTo(pivot) <= 0) {
                i++;
                T temp = data.get(i);
                data.set(i, data.get(j));
                data.set(j, temp);
            }
        }
        T temp = data.get(i + 1);
        data.set(i + 1, data.get(high));
        data.set(high, temp);
        return i + 1;
    }

    @Override public String name() { return "Quick Sort"; }
    @Override public String bestCase() { return "O(n log n)"; }
}

// Context that uses a SortStrategy
public class DataSorter<T extends Comparable<T>> {
    private SortStrategy<T> strategy;

    public DataSorter(SortStrategy<T> strategy) {
        this.strategy = strategy;
    }

    // Strategy can be swapped at RUNTIME
    public void setStrategy(SortStrategy<T> strategy) {
        this.strategy = strategy;
    }

    public List<T> sort(List<T> data) {
        List<T> copy = new ArrayList<>(data);
        long start = System.nanoTime();
        strategy.sort(copy);
        long duration = System.nanoTime() - start;
        System.out.printf("Sorted %d items using %s in %,d ns%n",
            data.size(), strategy.name(), duration);
        return copy;
    }
}

// ============== EXAMPLE 2: Payment Strategy ==============
public interface PaymentStrategy {
    PaymentResult pay(double amount, Map<String, String> details);
    boolean isApplicable(Map<String, String> context);
    String getStrategyName();
}

public class CreditCardStrategy implements PaymentStrategy {
    @Override
    public PaymentResult pay(double amount, Map<String, String> details) {
        String last4 = details.getOrDefault("cardLast4", "****");
        System.out.printf("[Credit Card ***%s] Charged $%.2f%n", last4, amount);
        return new PaymentResult(true, "CC-" + System.currentTimeMillis(), "Credit card payment OK");
    }

    @Override
    public boolean isApplicable(Map<String, String> context) {
        return context.containsKey("cardNumber");
    }

    @Override public String getStrategyName() { return "Credit Card"; }
}

public class PayPalStrategy implements PaymentStrategy {
    @Override
    public PaymentResult pay(double amount, Map<String, String> details) {
        String email = details.getOrDefault("paypalEmail", "user@paypal.com");
        System.out.printf("[PayPal: %s] Payment of $%.2f processed%n", email, amount);
        return new PaymentResult(true, "PP-" + System.currentTimeMillis(), "PayPal payment OK");
    }

    @Override
    public boolean isApplicable(Map<String, String> context) {
        return context.containsKey("paypalEmail");
    }

    @Override public String getStrategyName() { return "PayPal"; }
}

public class CryptoStrategy implements PaymentStrategy {
    private final double btcRate;

    public CryptoStrategy(double btcRate) { this.btcRate = btcRate; }

    @Override
    public PaymentResult pay(double amount, Map<String, String> details) {
        double btcAmount = amount / btcRate;
        String wallet = details.getOrDefault("walletAddress", "unknown");
        System.out.printf("[Bitcoin] Sent %.8f BTC (~$%.2f) to %s%n", btcAmount, amount, wallet);
        return new PaymentResult(true, "BTC-" + System.currentTimeMillis(),
            String.format("%.8f BTC transferred", btcAmount));
    }

    @Override
    public boolean isApplicable(Map<String, String> context) {
        return context.containsKey("walletAddress");
    }

    @Override public String getStrategyName() { return "Bitcoin"; }
}

// PaymentContext — uses strategies
public class ShoppingCart2 {
    private PaymentStrategy paymentStrategy;
    private final List<String> items = new ArrayList<>();
    private double total = 0;

    public void addItem(String item, double price) {
        items.add(item);
        total += price;
    }

    public void setPaymentStrategy(PaymentStrategy strategy) {
        this.paymentStrategy = strategy;
        System.out.println("Payment method set to: " + strategy.getStrategyName());
    }

    public PaymentResult checkout(Map<String, String> paymentDetails) {
        if (paymentStrategy == null) throw new IllegalStateException("No payment method selected");
        System.out.println("Checking out " + items.size() + " items for $" + total);
        return paymentStrategy.pay(total, paymentDetails);
    }

    // Auto-select strategy based on available details
    public void autoSelectStrategy(List<PaymentStrategy> strategies, Map<String, String> context) {
        strategies.stream()
            .filter(s -> s.isApplicable(context))
            .findFirst()
            .ifPresent(this::setPaymentStrategy);
    }
}

// ============== EXAMPLE 3: Discount Strategy ==============
@FunctionalInterface  // Can be implemented with lambdas!
public interface DiscountStrategy {
    double apply(double originalPrice);
}

public class DiscountCalculator {
    // Predefined strategies as static constants (strategy as enum-like)
    public static final DiscountStrategy NO_DISCOUNT = price -> price;
    public static final DiscountStrategy TEN_PERCENT = price -> price * 0.90;
    public static final DiscountStrategy TWENTY_PERCENT = price -> price * 0.80;
    public static final DiscountStrategy SENIOR_DISCOUNT = price -> price * 0.85;
    public static final DiscountStrategy EMPLOYEE_DISCOUNT = price -> price * 0.70;

    private DiscountStrategy strategy;

    public DiscountCalculator(DiscountStrategy strategy) {
        this.strategy = strategy;
    }

    public double calculate(double price) {
        return strategy.apply(price);
    }

    // Strategies can be COMPOSED (chained)
    public static DiscountStrategy combine(DiscountStrategy first, DiscountStrategy second) {
        return price -> second.apply(first.apply(price));
    }
}

public class StrategyPatternDemo {
    public static void main(String[] args) {
        // Sorting Strategy
        DataSorter<Integer> sorter = new DataSorter<>(new QuickSortStrategy<>());
        List<Integer> numbers = Arrays.asList(64, 34, 25, 12, 22, 11, 90);
        List<Integer> sorted = sorter.sort(numbers);
        System.out.println("Quick sorted: " + sorted);

        // Switch to bubble sort at runtime
        sorter.setStrategy(new BubbleSortStrategy<>());
        sorter.sort(numbers);

        // Payment Strategy
        ShoppingCart2 cart = new ShoppingCart2();
        cart.addItem("Laptop", 999.99);
        cart.addItem("Mouse", 29.99);

        // Pay with credit card
        cart.setPaymentStrategy(new CreditCardStrategy());
        Map<String, String> cardDetails = new HashMap<>();
        cardDetails.put("cardLast4", "4242");
        PaymentResult result = cart.checkout(cardDetails);
        System.out.println(result.message());

        // Discount Strategy using lambdas
        DiscountCalculator calc = new DiscountCalculator(DiscountCalculator.TEN_PERCENT);
        System.out.println("After 10% discount: $" + calc.calculate(100.0));

        // Composed strategy: 10% + 20% discount
        DiscountStrategy combined = DiscountCalculator.combine(
            DiscountCalculator.TEN_PERCENT,
            DiscountCalculator.TWENTY_PERCENT
        );
        calc = new DiscountCalculator(combined);
        System.out.println("After 10%+20% discount: $" + calc.calculate(100.0)); // $72

        // Custom strategy via lambda
        DiscountStrategy bulkDiscount = price -> price > 500 ? price * 0.75 : price * 0.95;
        calc = new DiscountCalculator(bulkDiscount);
        System.out.println("Bulk discount ($600): $" + calc.calculate(600.0)); // $450
    }
}
```

**Strategy vs Other Patterns:**
- **Strategy vs State**: Strategy changes behavior when explicitly set; State changes automatically when internal state changes
- **Strategy vs Template Method**: Strategy uses composition (inject algorithm); Template Method uses inheritance (override method)
- **Strategy vs Command**: Command encapsulates the *what to do*; Strategy encapsulates *how to do it*

**Benefits of Strategy:**
- ✅ Eliminates conditionals — no `if/else` or `switch` for algorithm selection
- ✅ Open/Closed — add new strategies without modifying context
- ✅ Swap algorithms at runtime
- ✅ Strategies are independently testable
- ✅ With `@FunctionalInterface` — can use lambda expressions as strategies

### 🇻🇳 Tiếng Việt

**Strategy Pattern** định nghĩa một họ thuật toán, đóng gói từng thuật toán, và làm chúng có thể hoán đổi nhau. Thuật toán có thể thay đổi độc lập với client sử dụng nó.

**Thành phần:**
- **Strategy interface**: Định nghĩa interface chung cho tất cả thuật toán
- **Concrete Strategies**: Mỗi class implement một thuật toán cụ thể
- **Context**: Giữ reference đến Strategy và delegate công việc

**Lợi ích:**
- Loại bỏ `if/else`, `switch` cho lựa chọn thuật toán
- Thêm strategy mới → không sửa Context (OCP)
- Thay đổi strategy lúc runtime
- Mỗi strategy dễ test độc lập
- Với `@FunctionalInterface` → dùng lambda làm strategy inline

**Ứng dụng thực tế:**
- Payment processing: credit card, PayPal, crypto
- Sorting: quick sort, merge sort, bubble sort
- Discount calculation: % discount, flat discount, loyalty discount
- Compression: gzip, zip, brotli
- Authentication: password, OAuth, JWT

---
## 🎓 Summary & Quick Reference

### OOP Pillars
| Pillar | Description | Java Keyword/Mechanism |
|--------|-------------|----------------------|
| Encapsulation | Bundle data + behavior, restrict access | `private`, getters/setters |
| Inheritance | Reuse parent class features | `extends` |
| Polymorphism | Many forms, runtime behavior | `@Override`, interfaces |
| Abstraction | Hide complexity, show interface | `abstract`, `interface` |

### SOLID Principles
| Principle | One-Liner |
|-----------|-----------|
| **S**ingle Responsibility | One class, one job |
| **O**pen/Closed | Extend without modifying |
| **L**iskov Substitution | Subtype substitutable for base |
| **I**nterface Segregation | Small, focused interfaces |
| **D**ependency Inversion | Depend on abstractions |

### Design Patterns Quick Reference
| Pattern | Type | Use When |
|---------|------|---------|
| Singleton | Creational | One instance globally needed |
| Factory | Creational | Object creation depends on runtime |
| Builder | Creational | Complex object with many optional params |
| Adapter | Structural | Incompatible interfaces need to work together |
| Bridge | Structural | Vary abstraction and implementation independently |
| Decorator | Structural | Add behavior without subclassing |
| Observer | Behavioral | One-to-many event notification |
| Strategy | Behavioral | Interchangeable algorithms |
| Command | Behavioral | Encapsulate actions, support undo/redo |
| Template Method | Behavioral | Define skeleton algorithm, vary steps |

---
*End of Document — 46 Questions Covered*

> 📝 **Note:** This guide uses Java 17+ syntax (records, pattern matching instanceof, text blocks). Some features like sealed classes and virtual threads (Java 21) are referenced where applicable.
>
> 🔗 **Further Reading:**
> - *Effective Java* by Joshua Bloch
> - *Clean Code* by Robert C. Martin
> - *Design Patterns* by Gang of Four (Gamma, Helm, Johnson, Vlissides)
> - *Refactoring* by Martin Fowler
