# Email setup

The page uses EmailJS to send the date plan by email.

## EmailJS

1. Create an account at emailjs.com.
2. Connect the email account that should send the date plan.
3. Create a template and set its **To Email** field to `niallcaley420@gmail.com` (or use `{{to_email}}`).
4. Copy the template ID shown beside the template name. It will look like `template_xxxxxxx`.
5. Put that template ID into `EMAILJS_TEMPLATE_ID` near the bottom of `Website.html`. The service ID and public key are already filled in.

The template should use these variables so the page can fill it automatically:

```text
Hi Niall,

Faye wants a date!

date: {{date}}
time: {{time}}
activities: {{activities}}
Bill: {{bill}}

thanks!
```

