
1. **DDL (데이터 정의 언어)**:

   DDL은 데이터베이스 구조를 정의하거나 변경하는 데 사용 

   - **테이블 생성**:

     ```sql
     CREATE TABLE Employees (
         EmployeeID INT PRIMARY KEY,
         FirstName VARCHAR(50),
         LastName VARCHAR(50),
         Department VARCHAR(50)
     );
     ```

   - **테이블 삭제**:

     ```sql
     DROP TABLE Employees;
     ```

2. **DML (데이터 조작 언어)**:

   DML은 데이터를 조회, 삽입, 수정 및 삭제하는 데 사용
   - **데이터 삽입**:

     ```sql
     INSERT INTO Employees (EmployeeID, FirstName, LastName, Department)
     VALUES (1, 'John', 'Doe', 'HR');
     ```

   - **데이터 조회**:

     ```sql
     SELECT FirstName, LastName FROM Employees WHERE Department = 'HR';
     ```

   - **데이터 수정**:

     ```sql
     UPDATE Employees SET Department = 'Finance' WHERE EmployeeID = 1;
     ```

   - **데이터 삭제**:

     ```sql
     DELETE FROM Employees WHERE EmployeeID = 1;
     ```

3. **DCL (데이터 제어 언어)**:

   DCL은 데이터베이스 사용 권한을 관리하는 데 사용

   - **권한 부여**:

     ```sql
     GRANT SELECT ON Employees TO User1;
     ```

   - **권한 취소**:

     ```sql
     REVOKE INSERT ON Employees FROM User2;
     ```

   - **트랜잭션 제어**:

     ```sql
     COMMIT; -- 변경사항을 확정짓습니다.
     ROLLBACK; -- 변경사항을 취소합니다.
     ```

각각의 SQL 문은 데이터베이스 작업을 다르게 처리하며, 데이터 정의, 조작 및 제어에 사용됩니다. 이러한 예제를 통해 데이터베이스 작업을 이해하고 적절한 SQL 문을 사용할 수 있을 것입니다.
