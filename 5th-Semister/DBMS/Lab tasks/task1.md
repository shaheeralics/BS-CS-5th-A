

### 1.1 Four Key Differences Between a File-Processing System and a DBMS

**1. Data Redundancy and Inconsistency**  
- **File-Processing System**: High levels of data redundancy, as the same data may be stored in multiple files across various departments or applications. This can lead to inconsistencies when updates are not synchronized across all files.  
  *Example*: If customer information is stored separately in both a sales and a billing file, any updates in one file may not reflect in the other, leading to data inconsistency.
- **DBMS**: Minimizes redundancy by storing data in a single, centralized database that can be accessed by multiple applications. Consistency is maintained as updates are made in a central location.
  *Example*: In a DBMS, customer information would be stored in one place, and all departments would access the same updated data, ensuring consistency.

**2. Data Access**  
- **File-Processing System**: Limited data access, typically restricted by specific, application-based code. Data retrieval often requires complex, manual coding for each type of request.
  *Example*: A simple query, like finding all customers in a specific city, might require custom code in a file-processing system, making access slower and more difficult.
- **DBMS**: Provides a robust, standardized query language, such as SQL, allowing efficient data access and manipulation. Users can execute complex queries without needing extensive code.
  *Example*: In a DBMS, retrieving customer data for a specific city can be done quickly using an SQL query like `SELECT * FROM Customers WHERE City = 'CityName'`.

**3. Data Integrity**  
- **File-Processing System**: Enforcing data integrity rules (like unique identifiers) is challenging as files operate in isolation. This can lead to errors and inconsistencies.
  *Example*: Without primary keys, duplicate customer records might exist in different files.
- **DBMS**: Enforces data integrity through constraints like primary keys, foreign keys, and other data validation rules, ensuring data accuracy.
  *Example*: A primary key constraint on a customer ID field ensures that each customer has a unique identifier, preventing duplicate records.

**4. Concurrency Control**  
- **File-Processing System**: Often lacks concurrency control or has limited support, making simultaneous data access difficult and potentially leading to data corruption.
  *Example*: If two users try to edit a record simultaneously, data conflicts may occur.
- **DBMS**: Supports concurrent access with various mechanisms like locking and transaction management, allowing multiple users to access and update data safely at the same time.
  *Example*: Multiple users can update records without conflict due to DBMS’s transaction control mechanisms, which ensure changes are processed in sequence.

---

### 1.2 Two Disadvantages of a Database System

**1. Complexity**  
- Database systems are complex to design, configure, and maintain. They require specialized skills for tasks like schema design, normalization, and performance optimization, making them challenging for general users.
  *Example*: Creating an optimized database structure often requires expertise in normalization principles, which can be difficult without training.

**2. Cost**  
- Database systems can be costly due to the need for powerful hardware, licensed software, and skilled personnel. Installation, regular maintenance, and data backup add to operational expenses.
  *Example*: Organizations may need to invest in server infrastructure and hire database administrators, which can be significant financial commitments, especially for smaller businesses.

---