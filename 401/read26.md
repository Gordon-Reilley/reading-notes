# Intro to Django

## Getting started with Django

- Deﬁne your data models entirely in Python. You get a rich, dynamic database-access API for free — but you can still write SQL if needed.

  ```python
    from django.db import models

    class Band(models.Model):
        """A model of a rock band."""
        name = models.CharField(max_length=200)
        can_rock = models.BooleanField(default=True)
    
    class Member(models.Model):
        """A model of a rock band member."""
        name = models.CharField("Member's name", max_length=200)
        instrument = models.CharField(choices=(
                ('g', "Guitar"),
                ('b', "Bass"),
                ('d', "Drums"),
            ),
            max_length=1
        )
        band = models.ForeignKey("Band")
  ```
- A clean, elegant URL scheme is an important detail in a high-quality web application. Django encourages beautiful URL design and doesn’t put any cruft in URLs, like .php or .asp. To design URLs for an application, you create a Python module called a URLconf. Like a table of contents for your app, it contains a simple mapping between URL patterns and your views.

  ```python
    from django.urls import path

    from . import views
    
    urlpatterns = [
        path('bands/', views.band_listing, name='band-list'),
        path('bands/<int:band_id>/', views.band_detail, name='band-detail'),
        path('bands/search/', views.band_search, name='band-search'),
    ]
          
    from django.shortcuts import render
    from bands.models import Band
    
    def band_listing(request):
        """A view of all bands."""
        bands = Band.objects.all()
        return render(request, 'bands/band_listing.html', {'bands': bands})

  ```
- Django’s template language is designed to strike a balance between power and ease. It’s designed to feel comfortable and easy-to-learn to those used to working with HTML, like designers and front-end developers. But it is also flexible and highly extensible, allowing developers to augment the template language as needed.

  ```python
    <html>
      <head>
        <title>Band Listing</title>
      </head>
      <body>
        <h1>All Bands</h1>
        <ul>
        {% for band in bands %}
          <li>
            <h2><a href="{{ band.get_absolute_url }}">{{ band.name }}</a></h2>
            {% if band.can_rock %}<p>This band can rock!</p>{% endif %}
          </li>
        {% endfor %}
        </ul>
      </body>
    </html>
  ```
- Django provides a powerful form library that handles rendering forms as HTML, validating user-submitted data, and converting that data to native Python types. Django also provides a way to generate forms from your existing models and use those forms to create and update data.

  ```python
    from django import forms
    
    class BandContactForm(forms.Form):
        subject = forms.CharField(max_length=100)
        message = forms.CharField()
        sender = forms.EmailField()
        cc_myself = forms.BooleanField(required=False)
  ```
- Django comes with a full-featured and secure authentication system. It handles user accounts, groups, permissions and cookie-based user sessions. This lets you easily build sites that allow users to create accounts and safely log in/out.

  ```python
    from django.contrib.auth.decorators import login_required
    from django.shortcuts import render
    
    @login_required
    def my_protected_view(request):
        """A view that can only be accessed by logged-in users"""
        return render(request, 'protected.html', {'current_user': request.user})
  ```
- One of the most powerful parts of Django is its automatic admin interface. It reads metadata in your models to provide a powerful and production-ready interface that content producers can immediately use to start managing content on your site. It’s easy to set up and provides many hooks for customization.

  ```python
    from django.contrib import admin
    from bands.models import Band, Member
    
    class MemberAdmin(admin.ModelAdmin):
        """Customize the look of the auto-generated admin for the Member model"""
        list_display = ('name', 'instrument')
        list_filter = ('band',)
    
    admin.site.register(Band)  # Use the default options
    admin.site.register(Member, MemberAdmin)  # Use the customized options
  ```
- Django offers full support for translating text into different languages, plus locale-specific formatting of dates, times, numbers, and time zones. It lets developers and template authors specify which parts of their apps should be translated or formatted for local languages and cultures, and it uses these hooks to localize web applications for particular users according to their preferences.

  ```python
    from django.shortcuts import render
    from django.utils.translation import gettext
    
    def homepage(request):
        """
        Shows the homepage with a welcome message that is translated in the
        user's language.
        """
        message = gettext('Welcome to our site!')
        return render(request, 'homepage.html', {'message': message})
  ```
- Django provides multiple protections against:

  - Clickjacking
  - Cross-site scripting
  - Cross Site Request Forgery (CSRF)
  - SQL injection
  - Remote code execution
### Things I want to know more about

- I would like to do more research on how the authentication in Django works because it sounds very intuitive.

### Sources

- <https://www.djangoproject.com/start/>
- <https://wsvincent.com/how-django-works-behind-the-scenes/>

[Back To Home](../README.md)