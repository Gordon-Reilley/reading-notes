# Permissions & Postgresql

## DRF Permissions

- Authentication or identification by itself is not usually sufficient to gain access to information or code. For that, the entity requesting access must have authorization.
- permissions determine whether a request should be granted or denied access
- Permission checks are always run at the very start of the view, before any other code is allowed to proceed
- Permission checks will typically use the authentication information in the request.user and request.auth properties to determine if the incoming request should be permitted.
- IsAuthenticated class in REST framework determines if access is allowed
- IsAuthenticatedOrReadOnly class in REST framework is less strict and allows read-only access
- Permissions in REST framework are always defined as a list of permission classes
- REST framework also allows for Object level permissions
- Object level permissions are used to determine if a user should be allowed to act on a particular object, which will typically be a model instance.
- If you're writing your own views and want to enforce object level permissions, or if you override the get_object method on a generic view, then you'll need to explicitly call the .check_object_permissions(request, obj) method on the view at the point at which you've retrieved the object.
- generic views will not automatically apply object level permissions API Reference
- AllowAny permission class will allow unrestricted access, regardless of if the request was authenticated or unauthenticated.
- The IsAuthenticated permission class will allow/deny permission to any unauthenticated user
- The IsAdminUser permission class will deny permission to any user, unless user.is_staff is True
- IsAuthenticatedOrReadOnly will allow authenticated users to perform any request. Requests for unauthorised users will only be permitted if the request method is one of the "safe" methods; GET, HEAD or OPTIONS.

### Things I want to know more about

- Excited to see how Permissions & Postgresql can build on an already awesome Django.

### Sources

- <https://www.django-rest-framework.org/api-guide/permissions/>
- <https://codefellows.github.io/common_curriculum/prework/SQL>

[Back To Home](../README.md)