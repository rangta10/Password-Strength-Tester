# Password-Strength-Tester

A Python utility that analyzes a password’s strength using regex-based criteria and assigns a score from 0-100, then classifies it as **Weak**, **Moderate**, or **Strong**.

---

##  Features
- Evaluates password length, character diversity (uppercase, lowercase, digits, symbols) and other patterns to assess strength.  
- Gives a numeric score (0-100) plus a qualitative grade (Weak/Moderate/Strong).  
- Simple CLI (command-line) interface to quickly test passwords.  
- Written in Python using the `re` library for regex checks.  
- Lightweight and easy to integrate or extend for other tools.

---

##  Getting Started
### Prerequisites
- Python 3.x installed on your system.  
- (Optional) A virtual environment recommended for isolating dependencies.

### Installation
```bash
git clone https://github.com/rangta10/Password-Strength-Tester.git  
cd Password-Strength-Tester  
# (Optional) Create and activate venv  
# python3 -m venv venv  
# source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt  # if you have any dependencies listed
```


You will be prompted to enter a password, after which you’ll receive a score and classification.
You can also import the module into your own script if you want to integrate its functionality.

 How It Works

Checks minimum and maximum length criteria.

Uses regex checks to detect presence of:

Lowercase letters

Uppercase letters

Digits

Symbols/special characters

Penalises for common weaknesses (for example: no diversity, repeated characters, easily guessable patterns).

Aggregates results into a single numeric score (0-100).

Maps the score to a grade:

Weak (0-40)

Moderate (41-70)

Strong (71-100)

 Example
```yaml
Enter a password: MyP@ssw0rd123  
Score: 78  
Classification: Strong  
```
 Why Use This Tool?

Quickly gauge how secure a password is from a diversity standpoint.

Can be used in scripts or applications to enforce stronger password policies.

Learn how simple regex-based checks can form part of a password-hardening strategy.

🛠 Extending & Customising

You may wish to:

Adjust scoring thresholds (e.g., what constitutes “Strong”).

Add checks for dictionary words or leaked passwords.

Integrate via a GUI or web interface.

Provide batch-mode support (test many passwords at once).

Log or export results for audit/tracking purposes.

 Project Structure
```
Password-Strength-Tester/
   ├── password_strength_tester.py     # Main script / module
   ├── README.md                        # This file
   ├── (optional) requirements.txt      # External dependencies
   └── (optional) tests/                # Unit tests you might add
```
 License

Choose an appropriate open-source license (e.g., MIT, Apache 2.0) and include a LICENSE file if you want to allow others to reuse the code.

 Contributions & Feedback

Feel free to submit pull requests, raise issues or suggest improvements. Any enhancements for usability, security checks or documentation are very welcome!

 Contact

If you have questions, ideas or want to collaborate further — get in touch via your GitHub profile or open an issue on the repository.

Enjoy using Password-Strength-Tester!
Happy coding & stay secure 
