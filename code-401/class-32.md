# Class 32

## Sources
- [DRF Permissions](https://www.django-rest-framework.org/api-guide/permissions/)
- [Review SQL Prework](https://codefellows.github.io/common_curriculum/prework/SQL)

## Bookmark and Review
- [Classy Django REST](https://www.cdrf.co/)
- [DRF Generic Views](https://www.django-rest-framework.org/api-guide/generic-views/)

## Reading Questions
[ChatGPT Prompt](https://chat.openai.com/c/e6bc7469-d7da-41bc-8b7f-26334979975e)
1. What are the key components and purpose of Django Rest Framework (DRF) permissions, and how do they help in securing an API?
> The permissions determine the level of access and permitted HTTP methods for different classes of users. Key components of DRF include Authentication, Permissions, Authorization, View-Level Permissions, and Object-Level Permissions. 
2. In SQL, what is the purpose of the SELECT statement, and how would you use it to retrieve all columns from a table called ‘employees’?
> A select statement is used to specify the column data or attributes. 
```SQL
FROM employees
SELECT *
```
3. Can you explain the role of DRF Generic Views and provide examples of their usage in building a RESTful API?
> Generic views is a set of pre-built views for common CRUD operations. They can be customized by overriding methods or attributes. 

```python
# ListView
from rest_framework.generics import ListAPIView
from .models import MyModel
from .serializers import MyModelSerializer

class MyModelListView(ListAPIView):
    queryset = MyModel.objects.all()
    serializer_class = MyModelSerializer
```

```python
# CreateView
from rest_framework.generics import CreateAPIView
from .models import MyModel
from .serializers import MyModelSerializer

class MyModelCreateView(CreateAPIView):
    queryset = MyModel.objects.all()
    serializer_class = MyModelSerializer
```

```python
# RetrieveView
from rest_framework.generics import RetrieveAPIView
from .models import MyModel
from .serializers import MyModelSerializer

class MyModelRetrieveView(RetrieveAPIView):
    queryset = MyModel.objects.all()
    serializer_class = MyModelSerializer
```

```python
# UpdateView
from rest_framework.generics import UpdateAPIView
from .models import MyModel
from .serializers import MyModelSerializer

class MyModelUpdateView(UpdateAPIView):
    queryset = MyModel.objects.all()
    serializer_class = MyModelSerializer
```

```python
# DeleteView
from rest_framework.generics import DestroyAPIView
from .models import MyModel
from .serializers import MyModelSerializer

class MyModelDestroyView(DestroyAPIView):
    queryset = MyModel.objects.all()
    serializer_class = MyModelSerializer
```

## Things I don't understand
- DRF