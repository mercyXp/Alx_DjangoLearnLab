# Create Operation

## Command
```python
from bookshelf.models import Book
book = Book.objects.create(title="1984", author="George Orwell", publication_year=1949)
book
```
## Expected Output
```python
<Book: Book object (1)>
# A new Book instance has been created in the database with ID=1.
```

