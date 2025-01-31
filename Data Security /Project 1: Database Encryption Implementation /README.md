**OVERVIEW**

This capstone project aims to demonstrate how to implement robust database encryption to protect sensitive data in a real-world system. Given the increasing threats to data security, encrypting data at rest and in transit is crucial for ensuring data confidentiality, integrity, and compliance with privacy regulations (such as GDPR, HIPAA, and others).
For this capstone project, the focus is on implementing:
- Transparent Data Encryption (TDE)
- Column-level encryption for a relational database system
- Ensuring secure communication using TLS/SSL.

**PROBLEM STATEMENT**

The task is securing a database that contains sensitive information (such as personally identifiable information or financial records). The database must be encrypted to prevent unauthorized access, while still ensuring the system’s performance is not significantly impacted.

**PROJECT OBJECTIVES**

1. **Implement Transparent Data Encryption (TDE):** Encrypt all data stored in the database to ensure data at rest is secure.
2. **Implement Column-Level Encryption:** Encrypt specific sensitive columns (e.g., social security numbers, credit card information) to ensure that only authorized users can decrypt and view them.
3. **Secure Data Transmission (TLS/SSL):** Secure database connections to prevent man-in-the-middle attacks during data transmission.
4. **Backup Encryption:** Ensure that backups are also encrypted to protect data off-site.
5. **User Access Control and Auditing:** Implement roles and permissions to restrict access to sensitive data and enable auditing.

**DATABASE SELECTION AND SETUP**

We will use SQL Server as the RDBMS, but the principles can be applied to other database systems like MySQL, Oracle, or PostgreSQL.
- **RDBMS:** Microsoft SQL Server (can use MySQL or PostgreSQL with similar encryption features).
- **Operating System:** Windows Server (but this can be adapted for Linux-based systems).
- **Encryption Tools:** SQL Server’s built-in Transparent Data Encryption (TDE) and Always Encrypted for column-level encryption.
- **Encryption Algorithm:** AES (Advanced Encryption Standard) for column-level encryption.

DESIGN AND ARCHITECTURE
**Transparent Data Encryption (TDE):**
- TDE will be used to encrypt the entire database at the storage level, ensuring that data is encrypted when stored on disk.
- The TDE encryption key is managed by SQL Server and automatically encrypts/decrypts data when read or written to the disk.
- The TDE setup will be applied to all databases within the SQL Server instance.

TDE SQL SERVER:
![image](https://github.com/user-attachments/assets/282a6a79-445d-43b0-9c5c-ec741e4df87a)

TDE AZURE SQL DATABASE:
