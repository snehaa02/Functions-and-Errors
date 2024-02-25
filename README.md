# Functions-and-Errors

This Solidity smart contract is called `StudentDatabase`. It allows users to create, view, update, and delete student profiles on the blockchain. Here's a breakdown of its key components:

- **Data Structure**: It defines a `struct` called `Student` to store information about each student, including their name, age, and technology stack.

- **Storage**: Student profiles are stored using a mapping called `students`, where each Ethereum address is mapped to a `Student` struct.

- **Functions**:
  - `createStudentProfile`: Allows users to create a new student profile with a name, age, and technology stack.
  - `confirmStudentName`, `confirmStudentAge`, `confirmStudentTechStack`: Allows users to confirm their name, age, and technology stack stored in the profile against provided values.
  - `updateProfile`: Allows users to update their existing student profile.
  - `deleteProfile`: Allows users to delete their student profile.
  - `viewProfile`: Allows users to view their own student profile.

- **Error Handling**: It defines a custom error `ProfileDoesNotExist` to handle cases where a profile is not found during deletion or viewing.

This contract aims to provide basic functionality for managing student profiles on the blockchain, ensuring data integrity and user control over their profiles.
