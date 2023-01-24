# Django Models

## Using Models

- Django web applications access and manage data through Python objects referred to as models.
- **Models** define the structure of stored data, including the field types and possibly also their maximum size, default values, selection list options, help text for documentation, label text for forms, etc. The definition of the model is independent of the underlying database — you can choose one of several as part of your project settings.
- Once you've chosen what database you want to use, you don't need to talk to it directly at all — you just write your model structure and other code, and Django handles all the dirty work of communicating with the database for you.
- We know that we need to store information about books (title, summary, author, written language, category, ISBN) and that we might have multiple copies available (with globally unique id, availability status, etc.). We might need to store more information about the author than just their name, and there might be multiple authors with the same or similar names. We want to be able to sort information based on book title, author, written language, and category.
- When designing your models, it makes sense to have separate models for every "object" (a group of related information). In this case, the obvious objects are books, book instances, and authors.
- You might also want to use models to represent selection-list options (e.g. like a drop down list of choices), rather than hard coding the choices into the website itself — this is recommended when all the options aren't known up front or may change.
- Obvious candidates for models, in this case, include the book genre (e.g. Science Fiction, French Poetry, etc.) and language (English, French, Japanese).
- Once we've decided on our models and field, we need to think about the relationships. Django allows you to define relationships that are one to one (OneToOneField), one to many (ForeignKey) and many to many (ManyToManyField).
- Models are usually defined in an application's **models.py** file. They are implemented as subclasses of `django.db.models.Model`, and can include fields, methods and metadata. The code fragment below shows a "typical" model, named `MyModelName`:

  ```python
    from django.db import models
    from django.urls import reverse
    
    class MyModelName(models.Model):
        """A typical class defining a model, derived from the Model class."""
    
        # Fields
        my_field_name = models.CharField(max_length=20, help_text='Enter field documentation')
        # …
    
        # Metadata
        class Meta:
            ordering = ['-my_field_name']
    
        # Methods
        def get_absolute_url(self):
            """Returns the URL to access a particular instance of MyModelName."""
            return reverse('model-detail-view', args=[str(self.id)])
    
        def __str__(self):
            """String for representing the MyModelName object (in Admin site etc.)."""
            return self.my_field_name
  ```
- The following common arguments can be used when declaring many/most of the different field types:
  - help_text: Provides a text label for HTML forms (e.g. in the admin site), as described above.
  - verbose_name: A human-readable name for the field used in field labels. If not specified, Django will infer the default verbose name from the field name.
  - default: The default value for the field. This can be a value or a callable object, in which case the object will be called every time a new record is created.
  - null: If True, Django will store blank values as NULL in the database for fields where this is appropriate (a CharField will instead store an empty string). The default is False.
  - blank: If True, the field is allowed to be blank in your forms. The default is False, which means that Django's form validation will force you to enter a value. This is often used with null=True, because if you're going to allow blank values, you also want the database to be able to represent them appropriately.
  - choices: A group of choices for this field. If this is provided, the default corresponding form widget will be a select box with these choices instead of the standard text field.
  - primary_key: If True, sets the current field as the primary key for the model (A primary key is a special database column designated to uniquely identify all the different table records). If no field is specified as the primary key, Django will automatically add a field for this purpose. The type of auto-created primary key fields can be specified for each app in AppConfig.default_auto_field or globally in the DEFAULT_AUTO_FIELD setting.
- The following list describes some of the more commonly used types of fields.
  - CharField is used to define short-to-mid sized fixed-length strings. You must specify the max_length of the data to be stored.
  - TextField is used for large arbitrary-length strings. You may specify a max_length for the field, but this is used only when the field is displayed in forms (it is not enforced at the database level).
  - IntegerField is a field for storing integer (whole number) values, and for validating entered values as integers in forms.
  - DateField and DateTimeField are used for storing/representing dates and date/time information (as Python datetime.date and datetime.datetime objects, respectively). These fields can additionally declare the (mutually exclusive) parameters auto_now=True (to set the field to the current date every time the model is saved), auto_now_add (to only set the date when the model is first created), and default (to set a default date that can be overridden by the user).
  - EmailField is used to store and validate email addresses.
  - FileField and ImageField are used to upload files and images respectively (the ImageField adds additional validation that the uploaded file is an image). These have parameters to define how and where the uploaded files are stored.
  - AutoField is a special type of IntegerField that automatically increments. A primary key of this type is automatically added to your model if you don't explicitly specify one.
  - ForeignKey is used to specify a one-to-many relationship to another database model (e.g. a car has one manufacturer, but a manufacturer can make many cars). The "one" side of the relationship is the model that contains the "key" (models containing a "foreign key" referring to that "key", are on the "many" side of such a relationship).
  - ManyToManyField is used to specify a many-to-many relationship (e.g. a book can have several genres, and each genre can contain several books). In our library app we will use these very similarly to ForeignKeys, but they can be used in more complicated ways to describe the relationships between groups. These have the parameter on_delete to define what happens when the associated record is deleted (e.g. a value of models.SET_NULL would set the value to NULL).

### Things I want to know more about

- I would like to do more research on Django admin features. They seem like they are very useful and a key skill to know when working with Django in the future.

### Sources

- <https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models>
- <https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Admin_site>

[Back To Home](../README.md)