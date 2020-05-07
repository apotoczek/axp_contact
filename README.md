# a NodeJS Contact Form App

Node server for processing contact forms from external sources

```html
<form method="post" action="http://example.com/contact@example.com">
  <input type="hidden" name="_subject" value="This is a test form" />
  <input type="email" name="_from" />
  <input type="text" name="first_name" />
  <input type="text" name="last_name" />
  <textarea name="comments"></textarea>
  <input type="submit" name="Submit" />
</form>
```

Fancier:

```html
<form method="post" action="http://my.mailgun.domain/my@email" enctype="multipart/form-data">
	<input type="hidden" name="_subject" value="This is a test form" />

	<label for="_from">Email</label>		<input type="email" name="_from" />			<br>
	<label for="first_name">First</label>	<input type="text" name="first_name" />		<br>
	<label for="last_name">Last</label>		<input type="text" name="last_name" />		<br>
	<label for="comments">Message</label>	<textarea name="comments"></textarea>		<br>
	<input type="file" name="_attachment" />											<br>
    <input type="submit" name="Submit" />
</form>
```

## Requirements

- Node.js v6.0.0 or greater.
- A Mailgun account.
