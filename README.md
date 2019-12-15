# DISIFY

Free email validation API. Check if disposable or temporary email address. Can be used both from website or implement for external use. 
API usage documentation included in website.

**Included validations**
- email and domain format
- internal database with blacklisted disposable email addresses (more than 30,000 domains included)
- DNS check for MX record existence
- internal database with blacklisted MX records (more than 100 providers included)
- SMTP response (under development)

**Features**
- Single email check
- Domain check
- Mass email/domain check (up to 10,000 unqiue records per request)
- Download valid email/domain list
- Responsive, easy to use both from desktop and mobile devices

**Website:** https://disify.com

*This is totally free service made just for passion. I hope its useful, enjoy!*

---

***Request example***

    GET https://disify.com/api/email/your@example.com

***Response example***

    { 
	    "format": true, 
	    "domain": "example.com", 
	    "disposable": false, 
	    "dns": true 
	}
