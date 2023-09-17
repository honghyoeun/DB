`ALTER`와 `INSERT`는 데이터베이스 관리 시스템(DBMS)에서 사용되는 SQL(Structured Query Language) 명령문

1. **ALTER (데이터 정의 언어 - DDL)**:
   - **목적**: `ALTER` 명령문은 데이터베이스 구조를 변경하는 데 사용. 테이블을 수정하거나 삭제하거나, 열을 추가, 수정 또는 삭제하는 데 사용
   - **예제**:

     ```sql
     -- 테이블에 새로운 열 추가
     ALTER TABLE Employees
     ADD COLUMN Salary DECIMAL(10, 2);

     -- 테이블의 열 수정
     ALTER TABLE Employees
     MODIFY COLUMN FirstName VARCHAR(100);

     -- 테이블 삭제
     DROP TABLE Employees;
     ```

2. **INSERT (데이터 조작 언어 - DML)**:
   - **목적**: `INSERT` 명령문은 데이터를 데이터베이스 테이블에 삽입하는 데 사용. 새로운 레코드(행)를 추가하거나, 기존 행의 데이터를 업데이트하지 않고 새로운 데이터를 테이블에 추가하는 데 사용
   - **예제**:

     ```sql
     -- 새로운 레코드(행) 삽입
     INSERT INTO Employees (EmployeeID, FirstName, LastName, Department)
     VALUES (1, 'John', 'Doe', 'HR');

     -- 테이블의 데이터 업데이트하지 않고 추가
     INSERT INTO Employees (EmployeeID, FirstName, LastName, Department)
     SELECT EmployeeID, FirstName, LastName, Department FROM NewEmployees;
     ```

요약하면, `ALTER`은 데이터베이스 구조를 변경하고 수정하는 데 사용되며, `INSERT`는 데이터를 데이터베이스 테이블에 추가하는 데 사용
