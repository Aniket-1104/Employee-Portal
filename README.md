# Employee-Portal



Steps to run Frontend: 
- open the project in vs code or any other
- open terminal
- cd to the project directory
- run "npm i" command to install the node modules
  <br>`npm i`
- run "npm start" to run the application
  <br>`npm start`
- search localhost:3000 to see the website

Steps to run Backend:
- open the project in inteliJ or any other ide
- go to application.properties under resources and change password to your MySQL password
- make sure to enter dummy data as provided in your MySql
- now run the EmployeePortalApplication file

MySql queries to run:
<br>
- -- Insert departments --<br>
`INSERT INTO department (department_name) VALUES
('Management'), ('Engineering'), ('Human Resources');`

- -- Insert managers --<br>
`INSERT INTO manager (manager_id, manager_name) VALUES
(1, 'John Doe'),
(2, 'Jane Smith'),
(3, 'Bob Johnson'),
(4, 'Alice Brown'),
(6, 'Eva White'),
(9, 'Max Turner'),
(10, 'Olivia Carter'),
(11, 'Leo Smith'),
(13, 'Mike Evans'),
(14, 'Lily Jones');`

- -- Insert employees --<br>
`INSERT INTO employees (name, date_of_birth, designation, email, phone_number, username, password, slack_url, personal_photo_link, office_photo_link, manager_id, department_id)
VALUES
('John Doe', '1980-01-01', 'CEO', 'john.doe@example.com', '1234567890', 'john_doe', 'password123', 'https://slack.com/johndoe', 'https://example.com/johndoe_photo', 'https://example.com/johndoe_office_photo', NULL, 1),
('Jane Smith', '1985-02-15', 'CTO', 'jane.smith@example.com', '9876543210', 'jane_smith', 'password456', 'https://slack.com/janesmith', 'https://example.com/janesmith_photo', 'https://example.com/janesmith_office_photo', 1, 2),
('Bob Johnson', '1990-05-20', 'HR Manager', 'bob.johnson@example.com', '5551234567', 'bob_johnson', 'password789', 'https://slack.com/bobjohnson', 'https://example.com/bobjohnson_photo', 'https://example.com/bobjohnson_office_photo', 1, 3),
('Alice Brown', '1992-08-10', 'SDE-3', 'alice.brown@example.com', '1112223333', 'alice_brown', 'passwordabc', 'https://slack.com/alicebrown', 'https://example.com/alicebrown_photo', 'https://example.com/alicebrown_office_photo', 2, 2),
('Charlie Green', '1995-03-25', 'SDE-2', 'charlie.green@example.com', '9998887777', 'charlie_green', 'passworddef', 'https://slack.com/charliegreen', 'https://example.com/charliegreen_photo', 'https://example.com/charliegreen_office_photo', 2, 2),
('Eva White', '1998-11-30', 'SDE', 'eva.white@example.com', '4445556666', 'eva_white', 'passwordeg', 'https://slack.com/evawhite', 'https://example.com/evawhite_photo', 'https://example.com/evawhite_office_photo', 2, 2),
('Sam Black', '2000-07-15', 'SDE-2', 'sam.black@example.com', '7778889999', 'sam_black', 'passwordhij', 'https://slack.com/samblack', 'https://example.com/samblack_photo', 'https://example.com/samblack_office_photo', 3, 2),
('Grace Miller', '1996-09-05', 'SDE', 'grace.miller@example.com', '3334445555', 'grace_miller', 'passwordklm', 'https://slack.com/gracemiller', 'https://example.com/gracemiller_photo', 'https://example.com/gracemiller_office_photo', 3, 2),
('Max Turner', '1994-04-18', 'Intern', 'max.turner@example.com', '6667778888', 'max_turner', 'passwordnop', 'https://slack.com/maxturner', 'https://example.com/maxturner_photo', 'https://example.com/maxturner_office_photo', 3, 2),
('Olivia Carter', '1997-12-12', 'Intern', 'olivia.carter@example.com', '2223334444', 'olivia_carter', 'passwordqrs', 'https://slack.com/oliviacarter', 'https://example.com/oliviacarter_photo', 'https://example.com/oliviacarter_office_photo', 4, 2),
('Leo Smith', '1993-06-28', 'SDE-3', 'leo.smith@example.com', '8889990000', 'leo_smith', 'passwordtuv', 'https://slack.com/leosmith', 'https://example.com/leosmith_photo', 'https://example.com/leosmith_office_photo', 6, 2),
('Sophie Taylor', '1991-10-08', 'SDE', 'sophie.taylor@example.com', '6661112222', 'sophie_taylor', 'passwordwxy', 'https://slack.com/sophietaylor', 'https://example.com/sophietaylor_photo', 'https://example.com/sophietaylor_office_photo', 9, 2),
('Mike Evans', '1988-07-20', 'SDE-2', 'mike.evans@example.com', '4440005555', 'mike_evans', 'passwordzab', 'https://slack.com/mikeevans', 'https://example.com/mikeevans_photo', 'https://example.com/mikeevans_office_photo', 10, 2),
('Lily Jones', '1987-04-15', 'HR Manager', 'lily.jones@example.com', '9990001111', 'lily_jones', 'passwordbcd', 'https://slack.com/lilyjones', 'https://example.com/lilyjones_photo', 'https://example.com/lilyjones_office_photo', 10, 3),
('Tom Wilson', '1986-01-30', 'Intern', 'tom.wilson@example.com', '1114447777', 'tom_wilson', 'passwordefg', 'https://slack.com/tomwilson', 'https://example.com/tomwilson_photo', 'https://example.com/tomwilson_office_photo', 11, 2),
('Emma Moore', '2001-02-12', 'Intern', 'emma.moore@example.com', '5556667777', 'emma_moore', 'passwordghij', 'https://slack.com/emmamoore', 'https://example.com/emmamoore_photo', 'https://example.com/emmamoore_office_photo', 11, 2),
('Ryan Clark', '1989-08-05', 'SDE-3', 'ryan.clark@example.com', '7778889999', 'ryan_clark', 'passwordijkl', 'https://slack.com/ryanclark', 'https://example.com/ryanclark_photo', 'https://example.com/ryanclark_office_photo', 13, 2),
('Zoe Anderson', '1999-05-22', 'SDE-2', 'zoe.anderson@example.com', '3334445555', 'zoe_anderson', 'passwordklmn', 'https://slack.com/zoeanderson', 'https://example.com/zoeanderson_photo', 'https://example.com/zoeanderson_office_photo', 13, 2),
('Oscar White', '1992-11-18', 'SDE', 'oscar.white@example.com', '8889990000', 'oscar_white', 'passwordopq', 'https://slack.com/oscarwhite', 'https://example.com/oscarwhite_photo', 'https://example.com/oscarwhite_office_photo', 14, 2);`


- -- Insert tags --<br>
`INSERT INTO tags (tag_name) VALUES
('Java'), ('JavaScript'), ('Python'), ('React'), ('Spring'), ('HR Policies'), ('Agile'), ('SQL'), ('Git'), ('Web Development');`

- -- Insert communities --<br>
`INSERT INTO communities (community_name, description) VALUES
('Engineering Team', 'Discussion about software development and engineering practices'),
('HR Forum', 'Discussion about human resources policies and practices'),
('Tech Enthusiasts', 'Community for sharing knowledge and ideas about technology');`

- -- Link tags to employees --<br>
`INSERT INTO employee_tags (employee_id, tag_id) VALUES
(1, 1), (1, 2), (2, 3), (3, 6), (4, 1), (4, 4), (5, 3), (6, 4),
(7, 2), (7, 5), (8, 5), (9, 9), (10, 7), (11, 8), (12, 8), (13, 1),
(14, 9), (15, 10), (16, 3), (17, 4), (18, 5), (19, 2);`

- -- Link communities to employees --<br>
`INSERT INTO employee_communities (employee_id, community_id) VALUES
(1, 1), (2, 1), (3, 2), (4, 2), (5, 1), (6, 1), (7, 1), (8, 1),
(9, 2), (10, 2), (11, 1), (12, 1), (13, 2), (14, 1), (15, 3), (16, 3),
(17, 1), (18, 1), (19, 3);`
