.. toctree::
   :hidden:
   :titlesonly:


Contact us / Ranger Mini Quote
===================================

We would love to hear from you and answer any product questions!


.. raw:: html
	
	<div class="dp-row">
		<div class="dp-col dp-col-12 dp-col-md-4 dp-col-lg-4">
			<span class="wpcf7-form-control-wrap your-name">
				<input type="text" id="userName" name="your-name" value size="40" class="wpcf7-form-form-control wpcf7-text wpcf7-validates-as-required" aria-required="true" aria-invalid="false" placeholder="Name*">
			</span>
		</div>
		<div class="dp-col dp-col-12 dp-col-md-4 dp-col-lg-4">
			<span class="wpcf7-form-control-wrap your-email">
				<input type="email" id="userEmail" name="your-email" value size="40" class="wpcf7-form-form-control wpcf7-email wpcf7-validates-as-required wpcf7-validates-as-email" aria-required="true" aria-invalid="false" placeholder="Email*">
			</span>
		</div>
		<div class="dp-col dp-col-12 dp-col-md-4 dp-col-lg-4">
			<span class="wpcf7-form-control-wrap your-phone">
				<input type="text" id="userPhone" name="your-phone" value size="40" class="wpcf7-form-form-control wpcf7-text wpcf7-validates-as-required" aria-required="true" aria-invalid="false" placeholder="Phone*">
			</span>
		</div>
	</div>


|

.. raw:: html

	<textarea rows cols id="inputString" style="width:100%;height:100px;">I am interested in information/prices on the Ranger Mini model and would like to know more about InDro Robotics products!</textarea>
	

|

.. raw:: html
	
	<button id="emailButton" class="btn primary" title onclick="sendEmail()">Send Email</button>
	<p id="demo">
	<script src="https://smtpjs.com/v3/smtp.js"></script>
	<script>
	
	function sendEmail() {
		
		userNameVar = document.getElementById("userName").value;
		userEmailVar = String(document.getElementById("userEmail").value);
		userPhoneVar = document.getElementById("userPhone").value;
		const userContentVar = String(document.getElementById("inputString").value) + "\n\n" + "Client Name: " + String(userNameVar) + ",\n" + "Client Phone: " + String(userPhoneVar) + ",\n" + "Client Email: " + String(userEmailVar);
		
		if(userContentVar!="" && userNameVar !="" && userEmailVar !="" && userPhoneVar !="")
		{
			try
			{
				document.getElementById("demo").innerHTML = "mail sent";
		      		Email.send({
				Host: "smtp.gmail.com",
				Username: "InDroDevelopment@gmail.com",
				Password: "publicPasswordIndro",
				To: 'InDroDevelopment@gmail.com',
				From: 'InDroDevelopment@gmail.com',
				Subject: "Email from Indro Documentation Site",
				Body: userContentVar,
		      		})
				.then(function (message) {alert("mail sent successfully")});
			}
			catch(e)
			{
				document.getElementById("demo").innerHTML = "email was unable to send";
			}
		}
		else
		{
			document.getElementById("demo").innerHTML = "missing input";
		}
	}
	</script>
	

|
|







