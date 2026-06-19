---
showRelatedContent: false
showReadingTime: false
showWordCount: false
showDate: false
showZenMode: false
showAuthor: false
showAuthorBottom: false
replyByEmail: false
showPagination: false
heroStyle: "background"
layoutBackgroundHeaderSpace: false
---
<div class="contact-form ">
<div class="extrone-profile ">
{{% markdown %}}
![Alt text](img/Profile_400x400.jpg)
# Extrone
{{% /markdown %}}
</div>
<form name="gform" id="gform"
    action="https://docs.google.com/forms/d/e/1FAIpQLScdKU-MISCXklCMYKa9vJP7lYq7YjGqS4P34YWhPEIx4pxybQ/formResponse?"
    target="hidden_iframe" onsubmit="submitted=true;">
    <div class="contact-field">
            <label class="required" for="name">
                {{< icon "tag" >}} Name
            </label>
        <input class="contact-form-input" type="text" id="entry.843253903" name="entry.843253903" placeholder="Your Name" required>
    </div>
    <div class="contact-field">
            <label class="required" for="email">
                {{< icon "email" >}} Email
            </label>
        <input class="contact-form-input" type="email" id="entry.1791357624" name="entry.1791357624" placeholder="Your Email" required>
    </div>
    <div class="contact-field">
            <label class="required" for="message">
                {{< icon "comment" >}} Message
            </label>
        <textarea class="contact-form-input" type="textarea" id="entry.183883436" name="entry.183883436" placeholder="Your Message" required></textarea>
        <!-- <div class="wrap">
            <div class="pull-tab">
                <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M0 20L20 0V12C20 16.4183 16.4183 20 12 20H0Z" fill="currentcolor"/>
                </svg>
            </div>
        </div> -->
    </div>
    <div class="contact-field">
        <div class="submit-button button">
            <input class="" type="submit" value="Send Message ">
            {{< icon "envelope" >}}
        </div>
    </div>
</form>
<div class="form-submit-confirmation modal" class="modal" id="form-submit-confirmation" style="visibility: hidden;">
    <div class="modal-window">
        <div class="modal-title-bar">
            <div class="modal-title">
                <h3>Message Sent!</h3>
            </div>
            <button class="modal-close-button button"> X </button>
        </div>
        <div class="modal-content" id="modal-content">
            <p>Thank you for contacting. I'll reach back to you as soon as possible.</p>
        </div>
    </div>
</div>
<iframe name="hidden_iframe" id="hidden_iframe" style="display:none;" onload="if(submitted) {
    var modal = document.getElementById('form-submit-confirmation');
    var button = document.getElementsByClassName('modal-close-button')[0];
    modal.style.display = 'flex';
    button.onclick = function() {
    modal.style.display = 'none';
    }
    window.onclick = function(event) {
    if (event.target == modal) {
        modal.style.display = 'none';
        }
    } 
    document.getElementById('gform').reset(); document.getElementById('form-submit-confirmation').style.visibility='visible';
    }">
</iframe>
</div>