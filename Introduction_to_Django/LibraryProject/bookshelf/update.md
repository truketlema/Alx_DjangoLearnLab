# Update Operation

```python
from bookshelf.models import Book
book = Book.objects.get(id=1)
book.title = "Nineteen Eighty-Four"
book.save()
Book.objects.get(id=1).title
```

Output:

'Nineteen Eighty-Four'
