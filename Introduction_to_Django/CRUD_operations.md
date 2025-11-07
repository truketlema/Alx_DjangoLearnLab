````markdown
# CRUD Operations for Book Model

## Create

```python
from bookshelf.models import Book
book = Book.objects.create(title="1984", author="George Orwell", publication_year=1949)
Book.objects.all()
```
````

**Output:**

```
<QuerySet [<Book: Book object (1)>]>
```

## Retrieve

```python
book = Book.objects.get(id=1)
book.title
book.author
book.publication_year
```

**Output:**

```
'1984'
'George Orwell'
1949
```

## Update

```python
book.title = "Nineteen Eighty-Four"
book.save()
Book.objects.get(id=1).title
```

**Output:**

```
'Nineteen Eighty-Four'
```

## Delete

```python
book.delete()
Book.objects.all()
```

**Output:**

```
<QuerySet []>
```

```

---

💡 **Tip:**

- Save this file in your `Introduction_to_Django` folder alongside your `bookshelf` app.
- You can also copy parts of it into `create.md`, `retrieve.md`, `update.md`, and `delete.md` if the activity requires separate files.

---

If you want, I can **also make ready-to-copy individual files** for `create.md`, `retrieve.md`, `update.md`, and `delete.md` so you’re fully covered. Do you want me to do that?
```
