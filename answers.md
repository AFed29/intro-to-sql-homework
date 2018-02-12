-- Return ALL the data in the 'movies' table.

SELECT * FROM movies;

-- Return ONLY the name column from the 'people' table

SELECT name FROM people;

-- Oops! Someone at CodeClan spelled Kate's name wrong! Change it to reflect the proper spelling (change 'Kte Preston' to 'Kate Preston').

UPDATE people
SET name = 'Kate Preston'
WHERE name = 'Kte Preston';

-- Return ONLY your name from the 'people' table.

SELECT name FROM people WHERE name = 'Alexander Fedenczuk';

-- The cinema is showing 'Batman Begins', but Batman is DC, not Marvel! Delete the entry from the 'movies' table.

DELETE FROM movies WHERE title = 'Batman Begins';

-- Create a new entry in the 'people' table with the name of one of the instructors.

INSERT INTO people (name) VALUES ('Finn Porter');

-- Jarrod Bennie, has decided to hijack our movie evening, Remove him from the table of people.

DELETE FROM people WHERE name = 'Jarrod Bennie';

-- The cinema has just heard that they will be holding an exclusive midnight showing of 'Guardians of the Galaxy 2'!! Create a new entry in the 'movies' table to reflect this.

INSERT INTO movies (title, year, show_time) VALUES ('Guardians of the Galaxy 2', 2017, '00:00');

-- The cinema would also like to make the Guardian movies a back to back feature. Update the 'Guardians of the Galaxy' show time from 18:55 to 21:30

UPDATE movies
SET show_time = '21:30'
WHERE title = 'Guardians of the Galaxy';
