# Week-10
Week 10 of CIS 213

CREATE TABLE listoftodos (
	id SERIAL, PRIMARY KEY,
	todo TEXT, NOT NULL
	isCompleted BOOLEAN DEFAULT false
);

SELECT * FROM listoftodos;

UPDATE listoftodos 
SET todo = ‘newTextOfTodo’
WHERE id = idOfTodo;

UPDATE listoftodos 
SET isCompleted = true;

INSERT INTO listoftodos
(id, todo, isCompleted)
VALUES
( DEFAULT, ‘textOfNewTodo’, false);

DELETE FROM listoftodos
WHERE id = idOfTodo;
