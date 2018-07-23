<template>
  <div>
    <div class="contact-header">
    </div>
    <ui-menu />
    <ui-layout container column>
			<ui-layout class="col-xs-12">
				<div class="contact-title"><h1>Kontaktujte nás</h1></div>
			</ui-layout>
			<ui-layout class="col-xs-12">
        <div class="contact-form">	       
      		<form name="contact" action="" method="post">
        		<label class="form-label" for="name">
          		Name:
        		</label>
        		<input class="form-field" name="name" id="name" />
        		<label class="form-label" for="email">
         		 Email:
        		</label>
        		<input class="form-field" name="email" id="email" />
        		<label class="form-label" for="message">
         		 Message:
        		</label>
        		<textarea class="form-field" name="message" id="message"></textarea>
        		<input class="form-button" type="submit" value="Send message" />
      		</form>
    		</div>
      </ui-layout>
    </ui-layout>
  	<ui-footer />   
  </div> 
</template>


<script>
import UiLayout from '~/components/UiLayout.vue'
import UiMenu from '~/components/UiMenu.vue'
import UiFooter from '~/components/UiFooter.vue'

export default {
  components: {
    UiLayout,
    UiFooter,
    UiMenu
  }
}

</script>

<style>

.contact-header{
	width: 100%;
	height: 300px;
	background-image: url("/assets/img/products.jpg");
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
}

.contact-title {
	margin:20px;
	padding-top: 60px;
	position:relative;
}

.contact-title::before {
	content: " ";
	background:#5383d3;
	width:10px;
  height:35px;
  left:-20px;
  position:absolute;
	
}

.contact-form {
    display: flex;
    align-items: top; /* Try changing this to center if you like it better! */
}

.contact-form label {
    min-width: 135px; /* Needs to be set to longest label (to keep inputs in a straight vertical line) */
    padding-right: 20px; /* This ensures a gap between label and input */
}


/* Set background color for entire form */
.contact-form {
    background-color: #eee;
}


/* Wrapper for all fields (not title) -- adding padding to make it line up with title (left) and keep it away from container edge */
.contact-form {
    padding-left: 20px;
    padding-right: 20px
}
.contact-form textarea {
    background-color: #ddd;
    border: none;
}

/* Button */
.contact-form .form-button {
    padding: 10px 20px 20px 0;
    text-align: right;
}

.contact-form .form-button[type=submit] {
    background-color: orange;
    color: white;
    padding: 10px 30px;
    letter-spacing: 4px;
    font-weight: normal;
    text-transform: uppercase;
}







</style>