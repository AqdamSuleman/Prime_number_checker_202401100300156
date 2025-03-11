# Prime_number_checker_202401100300156
Here’s a professional README.md file for your Prime Number Generator and Checker project:

markdown
Copy
Edit
# Prime Number Generator and Checker

This is a Python project that allows users to:  
✅ Check if a number is prime.  
✅ Generate a list of the first `n` prime numbers.  

---

## 🚀 Features
- Efficient prime number checking using trial division up to √n.  
- Fast prime number generation using a loop-based approach.  
- User-friendly interface with options to continue or exit.  

---

## 🛠️ Installation
1. **Clone the repository**:
```bash
git clone https://github.com/YourUsername/Prime-Number-Generator.git
Navigate to the project folder:
bash
Copy
Edit
cd Prime-Number-Generator
Run the Python file:
bash
Copy
Edit
python prime_number.py
📌 Usage
Run the program.
Choose one of the following options:
1 – Check if a number is prime.
2 – Generate a list of prime numbers.
3 – Exit the program.
Follow the on-screen instructions.
💻 Code Overview
Prime Checking Function
python
Copy
Edit
def is_prime(num):
    if num <= 1:
        return False
    for i in range(2, int(num**0.5) + 1):
        if num % i == 0:
            return False
    return True
Checks if a number is prime by testing divisibility up to √n.
Prime Generation Function
python
Copy
Edit
def generate_primes(n):
    primes = []
    num = 2
    while len(primes) < n:
        if is_prime(num):
            primes.append(num)
        num += 1
    return primes
Generates the first n prime numbers.
Main Function
python
Copy
Edit
def main():
    while True:
        print("\n1. Check if a number is prime")
        print("2. Generate a list of prime numbers")
        print("3. Exit")
        
        choice = input("Enter your choice (1/2/3): ")
        
        if choice == '1':
            num = int(input("Enter a number to check: "))
            if is_prime(num):
                print(f"{num} is a prime number.")
            else:
                print(f"{num} is not a prime number.")
            
            next_step = input("Do you want to continue? (yes/no): ").strip().lower()
            if next_step != 'yes':
                print("Exiting the program. Goodbye!")
                break
        
        elif choice == '2':
            n = int(input("How many prime numbers do you want to generate? "))
            primes = generate_primes(n)
            print(f"The first {n} prime numbers are: {primes}")
        
        elif choice == '3':
            print("Exiting the program. Goodbye!")
            break
        
        else:
            print("Invalid choice! Please try again.")

if __name__ == "__main__":
    main()
🌟 Example Output
Example 1: Checking a prime number

pgsql
Copy
Edit
Enter your choice (1/2/3): 1
Enter a number to check: 7
7 is a prime number.
Do you want to continue? (yes/no): no
Exiting the program. Goodbye!
Example 2: Generating prime numbers

java
Copy
Edit
Enter your choice (1/2/3): 2
How many prime numbers do you want to generate? 5
The first 5 prime numbers are: [2, 3, 5, 7, 11]
📝 Contributing
Feel free to fork the repository and submit a pull request.

🏆 Acknowledgements
Built using Python
Created by Aqdam
📃 License
This project is licensed under the MIT License.
See the LICENSE file for more details.

yaml
Copy
Edit

---

### 🔥 **What’s Included:**
✅ Clean format  
✅ Installation and usage instructions  
✅ Code overview  
✅ Example output  
✅ Contribution guidelines  
