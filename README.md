# Muscle
Repository for teacher task

#Создание тригера на заполнения таблицы logitable когда что-то добавят в таблицу autod
```
CREATE TRIGGER autoLisamine
at autod
FOR INSERT
An
INSERT INTO logitabel(toiming, aeg, autoAndmed)
SELECT 'AutoNumber on lisatud', GETDATE(), auto_nimetus FROM inserted
```

#Создание таблицы logitable
```
CREATE TOBLE IN logitabel {
	id int primary key identity(1,1),
	toiming varchar(200), 
	aeg datetime, 
	autoAndmed varchar(200)};
```

#В таблице users ГДЕ id равно 3 значение поля age станет 18, а country Эстония
```
UPDOTE users SETING age = '18' AND country = 'Эстония' WHERE id = '3';
```
