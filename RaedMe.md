Добавил сохранение данных в другом формате, для этого:
Добавил в класс UserMapper новое поле: separator, и изменил констукторы и методы для преобразования данных
Изменил класс DBConnector, заменил все статичексие методы на обычные, так как появилась необходимость сохранения данных в разных форматах и разных "БД". Добавил в него поле operation, и возможность создания экземпляров класса DBConnector при помощи уже существующих файловых операций. (впоследствии убрал)
Изменил конструкторы класса UserRepository
Добавил удаление данных из БД, для этого:
Реализовал в классе UserRepository соотв. метод из интерфейса
Добавил в класс UserView поведение при команде DELETE
Перенес в класс UserRepository и интерфейс GBRepository методы DAO (в метод write добавил поведение из метода saveAll, метод readAll для наглядности оставил как есть)