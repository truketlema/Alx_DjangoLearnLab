# Create Operation

```python
from bookshelf.models import Book
book = Book.objects.create(title="1984", author="George Orwell", publication_year=1949)
Book.objects.all()
```

Output:
<QuerySet [<Book: Book object (1)>]>
