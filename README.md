# text-input

<input>
The <input> element is used to create several different form controls. The value of the typeattribute determines what kind of input they will be creating.
type="text"
When the type attribute has a value of text, it creates a singleline text input.
name
When users enter information into a form, the server needs to know which form control each piece of data was entered into. (For example, in a login form, the server needs to know what has been entered as the username and what has been given as the password.) Therefore, each form control requires a name attribute. The value of this attribute 
identifies the form control and is sent along with the information they enter to the server.

size
The size attribute should not be used on new forms. It was used in older forms to indicate the width of the text input (measured by the number of characters that would be seen). For example, a value of 3 would create a box wide enough to display three characters (although a user could enter more characters if they desired).In any new forms you write, 
CSS should be used to control the width of form elements. The size attribute is only mentioned here because you may come across it when looking at older code.

maxlength
You can use the maxlength attribute to limit the number of characters a user may enter into the text field. Its value is the number of characters they may enter. For example, if you were asking for a year, the maxlength attribute could have a value of 4.

<form action="http://www.example.com/login.php">
  <p>Username:
    <input type="text" name="username" size="15" maxlength="30" />
  </p>
  <p>Password:
    <input type="password" name="password" size="15" maxlength="30" />
  </p>
</form>
