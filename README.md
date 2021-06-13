# Software-Engineering

### Software Engineering - Library Reservation System
***

1. Topic
2. Requirement analysis
3. System modeling
4. Architectural Design
5. Implementation
6. Testing
7. Members
***

1. Topic
* "Library Program"
* A program that systematically manages loans and returns for users. <br>
It allows librarians to manage libraries conveniently.<br>
This topic was selected to provide convenience and help users manage their books.
***

2. Requirement analysis
* Functional Requirement
* ![1](https://user-images.githubusercontent.com/67234937/121791889-ba85fa00-cc29-11eb-819d-6e25c288dde0.jpg)

* Non-functional Requirement
<br> a. Usability
<br> It will organize a simple UI so that users can see the program functions briefly. 
<br> In addition the server of the program will be built separately, reducing size and data of program.
<br><br> b. Reliability
<br> Programs used by users and administrators in this program are separated from each other.
<br> For the stability of the program we used a tool like Jmeter. This allowed us to test a lot of   
concurrent connections and constantly modify the code.
<br><br> c. Performance
<br> Searching for books and displaying search information should be done within 5 seconds. 
<br> In addition, the user’s information, book loan / return status, and changes in the book DB are   
immediately reflected on the database server.
***

3. System Modeling
* Scenarios
* <img width="395" alt="2" src="https://user-images.githubusercontent.com/67234937/121791957-54e63d80-cc2a-11eb-83c8-3cf0db7a1ef2.PNG">

* Interaction models
* ![3](https://user-images.githubusercontent.com/67234937/121791958-5a438800-cc2a-11eb-8817-21edf1e51f17.png)
* ![4](https://user-images.githubusercontent.com/67234937/121791959-5f083c00-cc2a-11eb-8974-198fb24f4630.png)

* Structure models
* ![5](https://user-images.githubusercontent.com/67234937/121791961-63ccf000-cc2a-11eb-9a26-592219340665.jpg)

* State model
* User <br> ![6](https://user-images.githubusercontent.com/67234937/121791965-67607700-cc2a-11eb-9b76-09869df16767.png)
* Administrator <br> ![7](https://user-images.githubusercontent.com/67234937/121791975-7b0bdd80-cc2a-11eb-8cf5-32548990002a.png)

***
4. Architecture Design
* ![8](https://user-images.githubusercontent.com/67234937/121791985-a0005080-cc2a-11eb-89b1-94dcced3344d.png)
* ![9](https://user-images.githubusercontent.com/67234937/121791990-a7275e80-cc2a-11eb-9242-5322eceaab94.png)

***
5. Implementation
* ## Android Studio + MySQL
* User <br> ![10](https://user-images.githubusercontent.com/67234937/121792060-89a6c480-cc2b-11eb-84c7-a000a1d292b4.gif)
* Administrator <br> ![11](https://user-images.githubusercontent.com/67234937/121792066-91666900-cc2b-11eb-8de7-83d225d49fe3.gif)

***
6. Testing
* Configuration Management
* SVN server (Visual SVN) <br> <img width="794" alt="SVN_server" src="https://user-images.githubusercontent.com/67234937/121792111-0df94780-cc2c-11eb-89ce-a96d936ea798.png">
* SVNList Server <br><img width="795" alt="SVNList_server" src="https://user-images.githubusercontent.com/67234937/121792112-12bdfb80-cc2c-11eb-9020-298f2a9e778b.png">
* Commit <br> <img width="960" alt="Commit" src="https://user-images.githubusercontent.com/67234937/121792119-1fdaea80-cc2c-11eb-9992-16ee935356e5.png">
* Code Line <br> <img width="959" alt="CodeLine" src="https://user-images.githubusercontent.com/67234937/121792116-1c476380-cc2c-11eb-89e3-6cc332477d57.png">
* Change Code Line <br> <img width="959" alt="ChangeCodeLine" src="https://user-images.githubusercontent.com/67234937/121792115-1782af80-cc2c-11eb-8ae5-530b25000176.png">

* Unit Testing
* <img width="344" alt="12" src="https://user-images.githubusercontent.com/67234937/121792156-6b8d9400-cc2c-11eb-8ba3-79f7254910a9.PNG">

* Test case Generation
* Directly entered code to check if functions are executed continuously in a specific situation
* <img width="960" alt="Test_case_code 액티비티들의 유기적인 기능들을 확인" src="https://user-images.githubusercontent.com/67234937/121792178-9841ab80-cc2c-11eb-9bc5-85c7c183769a.png">

* We had test without entering the code directly through the UI
* <img width="960" alt="Test case" src="https://user-images.githubusercontent.com/67234937/121792174-924bca80-cc2c-11eb-9795-a2e451093fd5.png">

* Notified when there is an error In a specific function or activity
* <img width="958" alt="로그인 오류" src="https://user-images.githubusercontent.com/67234937/121792188-b4454d00-cc2c-11eb-9111-b3b38c71866a.png">

* Test Coverage analysis
* <img width="375" alt="13" src="https://user-images.githubusercontent.com/67234937/121792194-cb843a80-cc2c-11eb-9563-22bc28704287.PNG">

* Performance Testing
* 10000 registered members at the same time
* <img width="894" alt="회원가입_10000명_1" src="https://user-images.githubusercontent.com/67234937/121792218-2322a600-cc2d-11eb-8ab8-21bf9c173c18.png">
* <img width="960" alt="회원가입_10000명_2" src="https://user-images.githubusercontent.com/67234937/121792219-287ff080-cc2d-11eb-8612-85db3894f691.png">

* 10000 login members at the same time
* <img width="893" alt="로그인_10000명_1" src="https://user-images.githubusercontent.com/67234937/121792235-5402db00-cc2d-11eb-868a-9ebe7cd8f129.png">
* <img width="894" alt="로그인_10000명_2" src="https://user-images.githubusercontent.com/67234937/121792234-4f3e2700-cc2d-11eb-8b50-bce098b0a3fd.png">

* 5000 books added at the same time
* <img width="894" alt="도서추가_5000명_1" src="https://user-images.githubusercontent.com/67234937/121792243-6aa93200-cc2d-11eb-9e86-b8a37bd07790.png">
* <img width="893" alt="도서추가_5000명_2" src="https://user-images.githubusercontent.com/67234937/121792241-654be780-cc2d-11eb-9260-ab94042ac952.png">

***
7. Members
* 심우석 (201636417)
* 박한음 (201835461)
* 전수환 (201835519)### Software Engineering - Library Reservation System
***

1. Topic
2. Requirement analysis
3. System modeling
4. Architectural Design
5. Implementation
6. Testing
7. Members
***

1. Topic
* "Library Program"
* A program that systematically manages loans and returns for users. <br>
It allows librarians to manage libraries conveniently.<br>
This topic was selected to provide convenience and help users manage their books.
***

2. Requirement analysis
* Functional Requirement
* ![1](https://user-images.githubusercontent.com/67234937/121791889-ba85fa00-cc29-11eb-819d-6e25c288dde0.jpg)

* Non-functional Requirement
<br> a. Usability
<br> It will organize a simple UI so that users can see the program functions briefly. 
<br> In addition the server of the program will be built separately, reducing size and data of program.
<br><br> b. Reliability
<br> Programs used by users and administrators in this program are separated from each other.
<br> For the stability of the program we used a tool like Jmeter. This allowed us to test a lot of   
concurrent connections and constantly modify the code.
<br><br> c. Performance
<br> Searching for books and displaying search information should be done within 5 seconds. 
<br> In addition, the user’s information, book loan / return status, and changes in the book DB are   
immediately reflected on the database server.
***

3. System Modeling
* Scenarios
* <img width="395" alt="2" src="https://user-images.githubusercontent.com/67234937/121791957-54e63d80-cc2a-11eb-83c8-3cf0db7a1ef2.PNG">

* Interaction models
* ![3](https://user-images.githubusercontent.com/67234937/121791958-5a438800-cc2a-11eb-8817-21edf1e51f17.png)
* ![4](https://user-images.githubusercontent.com/67234937/121791959-5f083c00-cc2a-11eb-8974-198fb24f4630.png)

* Structure models
* ![5](https://user-images.githubusercontent.com/67234937/121791961-63ccf000-cc2a-11eb-9a26-592219340665.jpg)

* State model
* User <br> ![6](https://user-images.githubusercontent.com/67234937/121791965-67607700-cc2a-11eb-9b76-09869df16767.png)
* Administrator <br> ![7](https://user-images.githubusercontent.com/67234937/121791975-7b0bdd80-cc2a-11eb-8cf5-32548990002a.png)

***
4. Architecture Design
* ![8](https://user-images.githubusercontent.com/67234937/121791985-a0005080-cc2a-11eb-89b1-94dcced3344d.png)
* ![9](https://user-images.githubusercontent.com/67234937/121791990-a7275e80-cc2a-11eb-9242-5322eceaab94.png)

***
5. Implementation
* ## Android Studio + MySQL
* User <br> ![10](https://user-images.githubusercontent.com/67234937/121792060-89a6c480-cc2b-11eb-84c7-a000a1d292b4.gif)
* Administrator <br> ![11](https://user-images.githubusercontent.com/67234937/121792066-91666900-cc2b-11eb-8de7-83d225d49fe3.gif)

***
6. Testing
* Configuration Management
* SVN server (Visual SVN) <br> <img width="794" alt="SVN_server" src="https://user-images.githubusercontent.com/67234937/121792111-0df94780-cc2c-11eb-89ce-a96d936ea798.png">
* SVNList Server <br><img width="795" alt="SVNList_server" src="https://user-images.githubusercontent.com/67234937/121792112-12bdfb80-cc2c-11eb-9020-298f2a9e778b.png">
* Commit <br> <img width="960" alt="Commit" src="https://user-images.githubusercontent.com/67234937/121792119-1fdaea80-cc2c-11eb-9992-16ee935356e5.png">
* Code Line <br> <img width="959" alt="CodeLine" src="https://user-images.githubusercontent.com/67234937/121792116-1c476380-cc2c-11eb-89e3-6cc332477d57.png">
* Change Code Line <br> <img width="959" alt="ChangeCodeLine" src="https://user-images.githubusercontent.com/67234937/121792115-1782af80-cc2c-11eb-8ae5-530b25000176.png">

* Unit Testing
* <img width="344" alt="12" src="https://user-images.githubusercontent.com/67234937/121792156-6b8d9400-cc2c-11eb-8ba3-79f7254910a9.PNG">

* Test case Generation
* Directly entered code to check if functions are executed continuously in a specific situation
* <img width="960" alt="Test_case_code 액티비티들의 유기적인 기능들을 확인" src="https://user-images.githubusercontent.com/67234937/121792178-9841ab80-cc2c-11eb-9bc5-85c7c183769a.png">

* We had test without entering the code directly through the UI
* <img width="960" alt="Test case" src="https://user-images.githubusercontent.com/67234937/121792174-924bca80-cc2c-11eb-9795-a2e451093fd5.png">

* Notified when there is an error In a specific function or activity
* <img width="958" alt="로그인 오류" src="https://user-images.githubusercontent.com/67234937/121792188-b4454d00-cc2c-11eb-9111-b3b38c71866a.png">

* Test Coverage analysis
* <img width="375" alt="13" src="https://user-images.githubusercontent.com/67234937/121792194-cb843a80-cc2c-11eb-9563-22bc28704287.PNG">

* Performance Testing
* 10000 registered members at the same time
* <img width="894" alt="회원가입_10000명_1" src="https://user-images.githubusercontent.com/67234937/121792218-2322a600-cc2d-11eb-8ab8-21bf9c173c18.png">
* <img width="960" alt="회원가입_10000명_2" src="https://user-images.githubusercontent.com/67234937/121792219-287ff080-cc2d-11eb-8612-85db3894f691.png">

* 10000 login members at the same time
* <img width="893" alt="로그인_10000명_1" src="https://user-images.githubusercontent.com/67234937/121792235-5402db00-cc2d-11eb-868a-9ebe7cd8f129.png">
* <img width="894" alt="로그인_10000명_2" src="https://user-images.githubusercontent.com/67234937/121792234-4f3e2700-cc2d-11eb-8b50-bce098b0a3fd.png">

* 5000 books added at the same time
* <img width="894" alt="도서추가_5000명_1" src="https://user-images.githubusercontent.com/67234937/121792243-6aa93200-cc2d-11eb-9e86-b8a37bd07790.png">
* <img width="893" alt="도서추가_5000명_2" src="https://user-images.githubusercontent.com/67234937/121792241-654be780-cc2d-11eb-9260-ab94042ac952.png">

***
7. Members
* 심우석 (201636417)
* 박한음 (201835461)
* 전수환 (201835519)
