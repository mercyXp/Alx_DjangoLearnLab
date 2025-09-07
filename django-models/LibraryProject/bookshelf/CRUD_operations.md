```bash
(env) PS D:\Alx_DjangoLearnLab\Introduction_to_Django\LibraryProject> python manage.py shell  
```
```python
7 objects imported automatically (use -v 2 for details).

Python 3.13.7 (tags/v3.13.7:bcee1c3, Aug 14 2025, 14:15:11) [MSC v.1944 64 bit (AMD64)] on win32
Type "help", "copyright", "credits" or "license" for more information.
(InteractiveConsole)

>>> from bookshelf.models import Book
>>> book = Book.objects.create(title="1984", author="George Orwell", publication_year=1949)
>>> book
<Book: Book object (1)>
>>> book = Book.objects.get(id=1)
>>> book.title, book.author, book.publication_year
('1984', 'George Orwell', 1949)
>>> book = Book.objects.get(id=1)
>>> book.title = "Nineteen Eighty-Four"
>>> book.save()
>>> book.title
'Nineteen Eighty-Four'
>>> book = Book.objects.get(id=1)
>>> book.delete()
(1, {'bookshelf.Book': 1})
>>> Book.objects.all()
<QuerySet []>
>>>
```