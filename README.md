<form>
   <label for="name">Name</label>
   <input type="text" id="name" name="name">

   <label for="email">Email</label>
   <input type="email" id="email" name="email">

   <label for="password">Password</label>
   <input type="password" id="password" name="password">

   <label for="dob">Date of Birth</label>
   <input type="date" id="dob" name="dob">

   <input type="checkbox" id="acceptTerms" name="acceptTerms">
   <label for="acceptTerms">Accept Terms & Conditions</label>

   <button type="submit">Submit</button>
</form>
function validateForm() {
  let x = document.forms["myForm"]["fname"].value;
  if (x == "") {
    alert("Name must be filled out");
    return false;
  }
}
<form name="myForm" action="/action_page.php" onsubmit="return validateForm()" method="post">
Name: <input type="text" name="fname">
<input type="submit" value="Submit">
</form>
