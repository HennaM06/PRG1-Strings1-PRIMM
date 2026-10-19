# Task 6: Paradigm Comparison, Answers

Complete this alongside `BRIEF_T6.md`.

## Guided comparison

### 1. Where is the data for a single book stored?

**Procedural version**

> In a dictionary. This stores the books title, author and checked_out status.

**Object-oriented version**

> In a book object. The book class stores the title, author and checked out status.

### 2. How is "check out a book" implemented?

**Procedural version**

> It is implemented by the function check_out_book (books,title). This loops through the books until it finds a book with the matching title with if book ["title"] == title and not book ["checked_out"]:then changing it directly affecting the dictionary 

**Object-oriented version**

> It has check_out_book(self,title) which searches through the books and, when finds the correct book calls book.check_out() this belongs to the book class and changes self checked out to true, changing its checkout status.

### 3. Trace: checking out an already checked-out book

**Procedural version**

> Because the status is already true, the condition is false. Meaning a copy will not be checked out again. The function carries on searching for another available matching book and if it doesn't it will return false.

**Object-oriented version**

> If that book is already checked out, not book.checked_out is false, so that copy isn't selected. It carries on searching for an available book with the same title.

### 4. Adding a new field, e.g. genre

**Procedural version**

> Add "genre" to the book dictionary in the add_book function 

**Object-oriented version**

> Add genre to book class and store it as self.genre. I would also need to pass the genre whena new book object is created 

## Written reflection

### 1. A genuine OOP advantage, for this specific problem

> OOP keeps the data and actions for a book together inside the book class.

### 2. A genuine procedural advantage, for this specific problem

> It is simpler as it uses more basic functions, dictionaries and a list meaning there are fewer classes/methods to understand. 

### 3. Which version would be easier to extend, and why?

> The OOP because related data and behaviour are grouped into classes.
