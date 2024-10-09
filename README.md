# Simple Database Management System

## Project Overview
This project is a **Simple Database Management System** (DBMS) implemented in C, designed to provide functionalities similar to a relational database. The core features include efficient data storage, retrieval, and manipulation using a **B+tree** structure for indexing. The system allows users to perform operations like inserting,  and searching for records efficiently.

## Key Features
- **B+tree Indexing**: Utilizes a B+tree data structure to maintain an index for fast data retrieval. This structure allows for efficient searches, insertions, and deletions while maintaining sorted order.
- **Dynamic Memory Management**: Implements memory management techniques to handle dynamic allocation and deallocation of memory for data storage, enhancing the performance and scalability of the database.
- **Row Structure**: Defines a `Row` structure to encapsulate the data stored in the database, including an ID, username, and email address.
- **Page Management**: Supports fixed-size pages for data storage, ensuring efficient utilization of memory and disk space, with a default page size of 4 KB (4096 bytes).
- **Cursor Implementation**: Provides a cursor for navigating through the B+tree, allowing for sequential access and manipulation of records.
- **Basic SQL-like Interface**: Implements a simple command-line interface to interact with the database, enabling users to perform CRUD (Create, Read, Update, Delete) operations.
- **Error Handling**: Incorporates error handling mechanisms to manage exceptions and ensure the integrity of data operations.

## Technical Details
- **Language**: C
- **Data Structure**: B+tree
- **Storage Format**: Key-value pairs stored in rows, indexed by their IDs.
- **Page Size**: Configurable page size of 4 KB (4096 bytes) for efficient storage management.
- **Memory Management**: Utilizes dynamic memory allocation to manage database records and tree nodes.

## Implementation Details
1. **Data Storage**: Records are stored as rows, and each row consists of an ID, username, and email. The B+tree structure indexes these records based on their IDs, allowing for quick lookups.
   
2. **B+tree Operations**:
   - **Insertion**: New records can be inserted into the database, and the B+tree structure automatically adjusts to accommodate these entries.
   - **Searching**: Users can search for records by ID, leveraging the B+tree’s efficient search capabilities.
  
3. **Cursor Functionality**: The cursor allows for easy navigation through the B+tree, enabling users to iterate over records, perform batch operations, and implement transaction-like behavior.

## Usage
To interact with the database:
- Compile the project using a C compiler.
- Run the executable to start the command-line interface.
- Use provided commands to perform CRUD operations:
  - **Insert** a new record.
  - **Update** an existing record by ID.


