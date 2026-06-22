# SQL-1
CREATE TABLE talabalar
(
    id       SERIAL PRIMARY KEY,
    ism      VARCHAR(50) NOT NULL,
    familiya VARCHAR(50) NOT NULL,
    yosh     INT,
    yonalish VARCHAR(100),
    ball     NUMERIC(4, 1)
);
INSERT INTO talabalar (ism, familiya, yosh, yonalish, ball)
VALUES ('Kamron', 'Aliyev', 20, 'Dasturlash', 85.0),
       ('Ogiloy', 'Karimova', 19, 'Ma''lumotlar ilmi', 92.5),
       ('Jasur', 'Umarov', 21, 'Kiberxavfsizlik', 78.0),
       ('Laylo', 'Sirojiddinova', 22, 'Dasturlash', 95.0),
       ('Dilshod', 'Hikmatov', 20, 'Sun''iy intellekt', 65.5),
       ('Damir', 'Tursunov', 23, 'Kiberxavfsizlik', 88.0),
       ('Zilola', 'Abduvaliyeva', 19, 'Dasturlash', 74.0),
       ('Temur', 'Xasanov', 21, 'Ma''lumotlar ilmi', 81.5),
       ('Gulbadan', 'Eshonqulova', 20, 'Sun''iy intellekt', 90.0),
       ('Gulbotir', 'Qodirov', 22, 'Dasturlash', 69.0);
SELECT *
FROM talabalar;
SELECT ism, familiya, ball
FROM talabalar;
SELECT ism AS talaba_ismi, yonalish AS fakulteti
FROM talabalar;
SELECT ism, familiya, ball AS joriy_ball, (ball * 1.1) AS yangi_ball
FROM talabalar;
SELECT ism, familiya, ball AS joriy_ball, (ball * 1.1) AS yangi_ball FROM talabalar;
