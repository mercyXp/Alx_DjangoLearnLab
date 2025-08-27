# Update Operation

## Command
```python
book = Book.objects.get(id=1)
book.title = "Nineteen Eighty-Four"
book.save()
book.title
```
## Expected Output
```python
'Nineteen Eighty-Four'
# Title has been updated successfully in the database.
```