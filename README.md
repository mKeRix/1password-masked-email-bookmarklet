# 1password-masked-email-bookmarklet

Occasionally, 1Password does not offer the [Masked Email](https://1password.com/fastmail/) dialog on web pages.
You could create addresses directly via the [Fastmail settings](https://app.fastmail.com/settings/masked), but then the additional integration functionality won't be available.
Instead, you can now use this handy bookmarklet to force the full Masked Email experience on any webpage.

## Usage

_If you are viewing this on github.com: the first step is required to be done from the [website](https://mkerix.github.io/1password-masked-email-bookmarklet/) instead_.

1. Add the link below into your browser favorites via drag and drop, right click or long tap on mobile.
   
   <a href="javascript: (() => {    const html = '<form><label for=&quot;email&quot; style=&quot;display: none;&quot;>Email</label><input id=&quot;op-masked-email-helper&quot; type=&quot;email&quot; name=&quot;email&quot; autocomplete=&quot;email&quot;><button type=&quot;submit&quot;>Submit</button></form>';    document.body.insertAdjacentHTML('afterbegin', html);    document.getElementById('op-masked-email-helper').focus();})();">1Password Masked Email Helper</a>
2. Click your bookmark while the page that you want to generate the email for is open.
3. From the newly added form, use the normal 1Password dialog to generate a Masked Email.
