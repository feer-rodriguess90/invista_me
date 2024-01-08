# Investment Tracker

## Overview
Investment Tracker is a web application built using Django 4.2.6 that allows users to manage their investments, such as computers, courses, books, and more. It provides features for viewing, adding, editing, and deleting investments. The project is designed with a user authentication system to ensure secure interactions.

## Usage
Visit the application in your web browser. <br />
<br />
Log in using your credentials or create a new account. <br />
<br />
Once logged in, you can: <br />
<br />
View a list of your investments at the '/investimentos/' URL. <br />
Add a new investment at the '/investimentos/criar/' URL. <br />
Edit an existing investment at the '/investimentos/editar/<investment_id>/' URL. <br />
Delete an existing investment at the '/investimentos/excluir/<investment_id>/' URL. <br />
<br />
## Code Explanation
Here's a brief explanation of the main components in the provided code: <br />
<br />
investimentos(request): Retrieves all investments from the database and renders them on the 'investimentos/investimentos.html' template. <br />
<br />
detalhe(request, id_investimento): Retrieves details of a specific investment and renders them on the 'investimentos/detalhe.html' template. <br />
<br />
criar(request): Handles the creation of a new investment. Uses the 'InvestimentoForm' form and redirects to the 'investimentos' page after successful submission. <br />
<br />
editar(request, id_investimento): Handles the editing of an existing investment. Uses the 'InvestimentoForm' form and redirects to the 'investimentos' page after successful submission. <br />
<br />
excluir(request, id_investimento): Handles the deletion of an existing investment. Displays a confirmation page before deleting the investment. <br />

## Dependencies
Django 4.2.6: A high-level Python web framework. <br />
Python 3.11.0: The programming language used for the project.

