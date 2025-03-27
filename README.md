# Задание 15. Исправить запрос на обновление
* Исправить запрос на обновление так, чтобы не сохранялась старая запись в БД, а у новой записи был id такой же как и у старой. Запрос необходимо исправить как для Person, так и для Message

* Классы должны располагаться следующим образом:

{корневой пакет}.controller.PersonController.java  
{корневой пакет}.repository.PersonRepository.java  
{корневой пакет}.dto.Person.java  
{корневой пакет}.controller.MessageController.java  
{корневой пакет}.repository.MessageRepository.java  
{корневой пакет}.dto.Message.java  
   
* Требования к API:

Person:

GET /person - Возврат списка объектов Person  
GET /person/{id} - Возврат объекта Person по id  
POST /person - Добавление объекта Person  
PUT /person/{id} - Изменение объекта Person по id  
DELETE /person/{id} - Удаление объекта Person по id  
Поля объекта Person:  

    int id;
    String firstname;
    String surname;
    String lastname;
    String birthday;
 
Message:

GET /message - Возврат списка объектов Message  
GET /message/{id} - Возврат объекта Message по id  
POST /message - Добавление объекта Message  
PUT /message/{id} - Изменение объекта Message по id  
DELETE /message/{id} - Удаление объекта Message по id  
Поля объекта Message:

    int id;
    String title;
    String text;
    LocalDateTime time;
