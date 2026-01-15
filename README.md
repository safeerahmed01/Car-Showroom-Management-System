# Car-Showroom-Management-System
A comprehensive Car Showroom Management System built with Java, demonstrating Object-Oriented Programming principles with a fully functional console interface, file persistence, and role-based access control.


🎯 Project Overview
This is a feature-rich Car Showroom Management System developed as a semester project to demonstrate core Java OOP concepts. The system provides a complete solution for managing car inventory, sales, customers, and employees through an intuitive console-based interface.

✨ **Key Feature**
👥 Role-Based Access Control
_**Admin:**___ Full system control - add/update/remove cars, approve worker applications, view reports
_**Worker:**___ Sell cars, track attendance, view personal sales statistics
**_Customer:_** Browse inventory, purchase cars, sell-back vehicles, view purchase history
_**Guest:**_ Browse and search cars without authentication

🚗 **Core Functionalities**
_Car Management:_ Complete CRUD operations with auto-generated IDs
_Sales System:_ Track sales with detailed records (customer, worker, price, timestamp)
_Worker Applications:_ Job application system with admin approval workflow
_Search & Filter:_ Advanced car search by name, brand, category, and price range
_Sorting:_ Multiple sorting options (price, name, quantity)
_Leaderboard:_ Worker performance tracking based on sales count
_File Persistence: _Automatic data save/load using Java Serialization
_Invoice Generation:_ Sales records appended to text files for easy tracking

🛠️ Technical Implementation
📚 OOP Principles Demonstrated
_Inheritance:_ Person → Admin/Worker/Customer
_Encapsulation:_ Private fields with public getters/setters
_Abstraction:_ Abstract Person class with menu() method
_Polymorphism:_ Method overriding in subclasses
_Generics:_ Custom Box<T> container class

🔧 Design Patterns & Concepts
_Factory Pattern:_ Static factory methods for object creation
_Singleton Pattern:_ Single Showroom instance management
_Composition: _Showroom contains collections of related objects
_Data Persistence:_ Object serialization for state management
_Exception Handling:_ Robust input validation and error handling

📁 Project Structure
text
CarShowroomSystem/
├── src/
│   ├── Main.java                 # Application entry point & CLI interface
│   ├── Showroom.java             # Core business logic & data management
│   ├── Person.java              # Abstract base class
│   ├── Admin.java               # Admin role implementation
│   ├── Worker.java              # Worker role with sales tracking
│   ├── Customer.java            # Customer functionality
│   ├── Car.java                 # Car entity with auto-ID generation
│   ├── SaleRecord.java          # Sales transaction records
│   ├── WorkerApplication.java   # Job application entity
│   ├── FileManager.java         # File I/O utilities
│   └── Box.java                # Generic container demonstration
├── data/
│   ├── showroom_data.bin       # Serialized application state
│   └── sales.txt              # Human-readable sales records
└── README.md                  # Project documentation

🎓 Educational Value
_This project serves as an excellent learning resource for:
Java beginners transitioning to intermediate level
Understanding real-world OOP implementation
File handling and serialization in Java
Console-based application design
Role-based system architecture
_
🚦 How to Run
bash
# Clone the repository
git clone https://github.com/yourusername/car-showroom-system.git

# Compile all Java files
javac *.java

# Run the application
java Main
📊 Sample Data Included
The system comes pre-loaded with sample data:

3 Cars (Honda Civic, Toyota Corolla, Tesla Model 3)

2 Workers (Ali, Basit)

1 Customer (Saad)

Default Admin credentials (admin/admin123)

🔍 Code Quality Highlights
Clean, documented code with JavaDoc-style comments

Consistent naming conventions

Modular design for easy extension

Comprehensive error handling

Memory-efficient collections usage

🔄 Future Enhancements
Potential improvements include:

Database integration (MySQL/PostgreSQL)

Graphical User Interface (JavaFX/Swing)

Email/SMS notifications

Advanced reporting with charts

Multi-branch showroom support

REST API for web/mobile access

