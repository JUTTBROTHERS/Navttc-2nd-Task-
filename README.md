<!DOCTYPE html>
<html>
<body>

<p>I am Internal Text</p>

<!-- I am Comment -->

<div id="includedContent"></div>

<script>
window.onload = function() {
  fetch('IIncluded.html')
    .then(response => response.text())
    .then(data => {
      document.getElementById('includedContent').innerHTML = data;
    });
};
</script>

</body>
</html>
