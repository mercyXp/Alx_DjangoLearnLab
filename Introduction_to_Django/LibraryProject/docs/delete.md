# Delete Operation

## Command
```python
book = Book.objects.get(id=1)
book.delete()
Book.objects.all()
```
## Expected Output
```python
(1, {'bookshelf.Book': 1})
# The book instance was deleted (1 record affected).

<QuerySet []>
# Confirmed: No books found in the database.
```