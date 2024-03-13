CREATE TABLE Coupon(ID SERIAL PRIMARY KEY,
	ProductName VARCHAR(24) NOT NULL,
	Description TEXT,
	Amount INT);

INSERT INTO Coupon (ProductName, Description, Amount) VALUES ('Caderno', 'Caderno Esperial', 5)

INSERT INTO Coupon (ProductName, Description, Amount) VALUES ('Caneta', 'Caneta Esferográfica', 2)

SELECT  * FROM  Coupon