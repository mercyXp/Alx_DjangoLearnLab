# Retrieve Operation

## Command
```python
book = Book.objects.get(id=1)
book.title, book.author, book.publication_year
```
## Expected Output
```python
('1984', 'George Orwell', 1949)
# Retrieved the book successfully with all its attributes.
```