## Django CRUD and Forms

- An HTML Form is a group of one or more fields/widgets on a web page, which can be used to collect information from users for submission to a server. Forms are a flexible mechanism for collecting user input because there are suitable widgets for entering many different types of data, including text boxes, checkboxes, radio buttons, date pickers and so on. Forms are also a relatively secure way of sharing data with the server, as they allow us to send data in POST requests with cross-site request forgery protection.

- While we haven't created any forms in this tutorial so far, we've already encountered them in the Django Admin site — for example, the screenshot below shows a form for editing one of our Book models, comprised of a number of selection lists and text editors.

### HTML Forms

<form action="/team_name_url/" method="post">
    <label for="team_name">Enter name: </label>
    <input id="team_name" type="text" name="name_field" value="Default name for team.">
    <input type="submit" value="OK">
</form>

- The submit input will be displayed as a button (by default) that can be pressed by the user to upload the data in all the other input elements in the form to the server (in this case, just the team_name). The form attributes define the HTTP method used to send the data and the destination of the data on the server (action):

- action: The resource/URL where data is to be sent for processing when the form is submitted. If this is not set (or set to an empty string), then the form will be submitted back to the current page URL. method: The HTTP method used to send the data: post or get. The POST method should always be used if the data is going to result in a change to the server's database because this can be made more resistant to cross-site forgery request attacks. The GET method should only be used for forms that don't change user data (e.g. a search form). It is recommended for when you want to be able to bookmark or share the URL.
 

- Django's form handling uses all of the same techniques that we learned about in previous tutorials (for displaying information about our models): the view gets a request, performs any actions required including reading data from the models, then generates and returns an HTML page (from a template, into which we pass a context containing the data to be displayed). What makes things more complicated is that the server also needs to be able to process data provided by the user, and redisplay the page if there are any errors.

- he arguments that are common to most fields are listed below (these have sensible default values):

    - required: If True, the field may not be left blank or given a None value. Fields are required by default, so you would set required=False to allow blank values in the form.

    - label: The label to use when rendering the field in HTML. If a label is not specified, Django will create one from the field name by capitalizing the first letter and replacing underscores with spaces (e.g. Renewal date).

    - label_suffix: By default, a colon is displayed after the label (e.g. Renewal date:). This argument allows you to specify a different suffix containing other characters (s).

    - initial: The initial value for the field when the form is displayed.

    - widget: The display widget to use.

    - help_text (as seen in the example above): Additional text that can be displayed in forms to explain how to use the field.

    - error_messages: A list of error messages for the field. You can override these with your own messages if needed.

    - validators: A list of functions that will be called on the field when it is validated.

    - localize: Enables the localization of form data input (see link for more information).

    - disabled: The field is displayed but its value cannot be edited if this is True. The default is False.

### Handling Forms

- The Form class is the heart of Django’s form handling system. It specifies the fields in the form, their layout, display widgets, labels, initial values, valid values, and (once validated) the error messages associated with invalid fields. The class also provides methods for rendering itself in templates using predefined formats (tables, lists, etc.) or for getting the value of any element (enabling fine-grained manual rendering).
- Declaring a Form

> from django import forms

> class class_name(forms.Form):
    

- Form fields

    BooleanField
    CharField
    ChoiceField
    TypedChoiceField
    DateField
    DateTimeField
    DecimalField
    DurationField
    EmailField
    FileField
    FilePathField
    FloatField
    ImageField


- Validation

    - Django provides numerous places where you can validate your data. The easiest way to validate a single field is to override the method clean_() for the field you want to check.
- URL configuration

    - urlpatterns += [
    path('put/the/path/here', add_the_view_here, name='view name')
   ]

- View

    - The view has to render the default form when it is first called and then either re-render it with error messages if the data is invalid, or process the data and redirect to a new page if the data is valid. In order to perform these different actions, the view has to be able to know whether it is being called for the first time to render the default form, or a subsequent time to validate data. For forms that use a POST request to submit information to the server, the most common pattern is for the view to test against the POST request type (if request.method == ‘POST’) to identify form validation requests and GET (using an else condition) to identify the initial form creation request. If you want to submit your data using a GET request, then a typical approach for identifying whether this is the first or subsequent view invocation is to read the form data (e.g. to read a hidden value in the form).
- Templating

    -The last step is templating in an html file, and it is same to the previous labs, as it uses liquid_tag and we add the form and input tags inside this file.

 