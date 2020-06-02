+++
fragment = "contact"
#disabled = true
date = "06-02-2020"
weight = 200
background = "success"
form_name = "defaultContact"

#title = "Contact Form"
#subtitle  = "*not working on demo page*"

# PostURL can be used with backends such as mailout from caddy
post_url = "https://example.com/mailout" #default: formspree.io
email = "mail@example.com"
button = "Send Button" # defaults to theme default 
netlify = true

# Optional google captcha
#[recaptcha]
#  sitekey = ""

[message]
  success = "Thank you for contacting us!" # defaults to theme default
  #error = "" # defaults to theme default

# Only defined fields are shown in contact form
[fields.name]
  text = "Your Name *"
  #error = "" # defaults to theme default

[fields.email]
  text = "Your Email *"
  #error = "" # defaults to theme default

[fields.phone]
  text = "Your Phone *"
  #error = "" # defaults to theme default

[fields.message]
  text = "Your Message *"
  #error = "" # defaults to theme default

# Optional hidden form fields
# Fields "page" and "site" will be autofilled
[[fields.hidden]]
  name = "page"

[[fields.hidden]]
  name = "someID"
  value = "example.com"
+++
