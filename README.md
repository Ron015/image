image url
# Example with Copy Button

This is an example of a code snippet with a copy button:

```html
<div id="code-container">
    <code>
        &lt;h1&gt;Hello, world!&lt;/h1&gt;
    </code>
    <button onclick="copyCode()">Copy</button>
</div>

<script>
    function copyCode() {
        var code = document.querySelector('#code-container code').textContent;
        navigator.clipboard.writeText(code).then(function() {
            alert('Code copied to clipboard!');
        }).catch(function(err) {
            alert('Failed to copy code: ', err);
        });
    }
</script>
```
