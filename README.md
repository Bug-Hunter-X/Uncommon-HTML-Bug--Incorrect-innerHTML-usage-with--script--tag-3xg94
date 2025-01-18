# Uncommon HTML Bug: innerHTML and Script Tag Injection

This repository demonstrates an uncommon HTML bug related to the improper use of `innerHTML` to inject a `<script>` tag.  This practice can lead to unexpected behavior, errors, and potential Cross-Site Scripting (XSS) vulnerabilities.

The `bug.html` file contains the buggy code. The `bugSolution.html` file shows the corrected approach.

**Bug:** Incorrectly appending a `<script>` tag using `innerHTML` can cause errors and unexpected behavior in Javascript.

**Solution:** Use `createElement()` instead of directly injecting the script tag through innerHTML.