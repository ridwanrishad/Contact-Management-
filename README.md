# Contact Management System (CMS)

The **Contact Management System (CMS)** is a command-line application built in Python designed to help users securely store, organize, and manage their personal or professional contacts. The application features a built-in user authentication system so multiple users can maintain isolated access, along with strict input validation to guarantee data integrity.


* **User Authentication:** Secure login and registration system (`users.txt`) to protect user directories.
* **Strict Input Validation:** Enforces digit-only validation for phone numbers to prevent formatting errors.
* **CRUD Operations:** Easily Add, View, Search, and Delete contacts.
* **Persistent Storage:** Data is automatically saved to local text files (`users.txt` and `contacts.txt`), ensuring no data is lost upon exit.
* **Modular Architecture:** Clean separation of concerns across multiple files (`main.py`, `auth.py`, `contact_operations.py`, `contact_storage.py`, `user_storage.py`, and `config.py`).


* **Language:** Python 3.x
* **Standard Libraries:** 
  * `os` (for checking file paths and managing storage)
  * `sys` (for controlled application exit)
* **Data Persistence:** Plain text files with custom parsing (`.txt`)


1. **Download & Extract:**
   Download and extract all the project modules into a single working directory:
   * `main.py`
   * `auth.py`
   * `contact_operations.py`
   * `contact_storage.py`
   * `user_storage.py`
   * `config.py`

2. **Open Terminal / Command Prompt:**
   Navigate to the directory where your project files are saved:
   ```bash
   cd path/to/your/project-folder
   ```

3. **Run the Application:**
   Execute the main entry point script using Python:
   ```bash
   python main.py
   ```


Follow these steps to test the full functionality of the application:

1. **Authentication Stage:**
   * When you run the script, the authentication menu will appear:
     ```text
     === Authentication ===
     1. Login
     2. Register
     ```
   * Choose **`2`** to register a new username and password. 
   * Once registered, restart or use your new credentials to **Login** (`1`).

2. **Adding a Contact:**
   * After a successful login, choose option **`1` (Add Contact)**.
   * Enter a name.
   * Enter a phone number. *Test the validation by typing letters (e.g., "abc")—the system will block it and prompt you until you enter digits only.*
   * Provide an optional email and address.

3. **Viewing & Searching Contacts:**
   * Choose option **`2` (View Contacts)** to see a neatly formatted list of your entries.
   * Choose option **`3` (Search Contact)** and enter the phone number to retrieve specific contact details.

4. **Deleting Contacts:**
   * Choose option **`4` (Delete Contact)** and enter the phone number of the contact you wish to remove.

5. **Exiting:**
   * Choose option **`5` (Exit)** to safely close the program.
