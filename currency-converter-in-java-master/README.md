# currency-converter-in-java


Currency converter (or currency exchange) is a mini project coded in Java programming language. This simple application provides a web-based interface for exchanging/converting money from one currency (say $) to another currency (say €).

The complete source code of currency exchange application can be downloaded from the link below. As this is just a mini project, project report and documentation are not available. You can go through the description below for project abstract.

Currency Converter Project Abstract:
Different countries use different currency, and there is daily variation in these currencies relative to one another. Those who transfer money from one country to another (one currency to another) must be updated with the latest currency exchange rates in the market.

Currency converter mini project is built keeping this thing in mind. It is simply a calculator-like app developed using Ajax, Java servlets web features. In this application, there is regular update about currency of every country by which it displays present currency market value and conversion rate.

Such application can be used by any user, but it is mainly useful for business, shares, and finance related areas where money transfer and currency exchange takes place on a daily basis.

In this currency converter app, users are provided with an option to select the type of conversion, i.e. from “this” currency to “that” currency. This simple feature allows users to enter amount to be converted (say currency in Dollars), and display the converted amount (say currency in Euro).



visit more projects - https://projectworlds.in

demo- https://www.projectworlds.in/java-projects-with-source-code/currency-converter-java-mini-project/
### System Architecture

#### High-Level Design and Structure

1. *Main Components:*
   - *CurrencyConverter (Main Class):*
     - *Function:* The main entry point of the application. It initializes the graphical user interface (GUI) and launches the main window.
     - *Interaction:* Calls MainWindow to display the main interface.

   - *MainWindow (Main Window Class):*
     - *Function:* The main window of the application that displays the user interface.
     - *Interaction:* Interacts with the user and displays various components such as buttons and text fields.

   - *AboutWindow (About Window Class):*
     - *Function:* A window that displays information about the application, such as the author, license, and version.
     - *Interaction:* Interacts with the user by displaying information and clickable links.

   - *Currency (Currency Class):*
     - *Function:* Represents a currency object containing information such as name, short name, and exchange values.
     - *Interaction:* Used to store and retrieve exchange values and perform currency conversions.

   - *JTextFieldLimit (Text Field Limit Class):*
     - *Function:* Limits the number of characters allowed in a text field, with an option to convert text to uppercase.
     - *Interaction:* Used in text fields to ensure correct data input.

2. *Interactions Between Components:*
   - *CurrencyConverter* initializes the GUI by calling MainWindow.
   - *MainWindow* displays the main interface and interacts with the user. It can call AboutWindow to display information about the application.
   - *AboutWindow* displays information about the application and interacts with the user through clickable links.
   - *Currency* objects are used to store and retrieve exchange values and perform currency conversions.
   - *JTextFieldLimit* is used in text fields to ensure correct data input.

3. *Data Flow:*
   - When the application starts, CurrencyConverter initializes the GUI and displays MainWindow.
   - The user interacts with MainWindow, which can access AboutWindow to display application information.
   - Currency objects are used to store and retrieve exchange values and perform conversions.
   - JTextFieldLimit ensures correct data input in text fields.

### System Architecture Tree


CurrencyConverter (Main Class)
│
├── MainWindow (Main Window Class)
│   │
│   ├── Currency (Currency Class)
│   │   ├── name
│   │   ├── shortName
│   │   └── exchangeValues
│   │
│   ├── JTextFieldLimit (Text Field Limit Class)
│   │   └── limit
│   │
│   └── AboutWindow (About Window Class)
│       ├── lblTitle
│       ├── lblLicenceMit
│       ├── lblVersion
│       ├── lblAuthor
│       └── lblLink
│
└── Logger (Logging Class)
    └── FileHandler


This tree structure visually represents the main components of your system and their relationships.

