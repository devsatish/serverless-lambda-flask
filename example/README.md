// example.ts

// Define an interface for a User
interface User {
    id: number;
    name: string;
    email: string;
}

// Create a class that implements the User interface
class UserAccount implements User {
    id: number;
    name: string;
    email: string;

    constructor(id: number, name: string, email: string) {
        this.id = id;
        this.name = name;
        this.email = email;
    }

    // Method to display user details
    displayUser(): void {
        console.log(`User ID: ${this.id}, Name: ${this.name}, Email: ${this.email}`);
    }
}

// Create a new user instance
const user = new UserAccount(1, "John Doe", "john.doe@example.com");

// Display the user details
user.displayUser();