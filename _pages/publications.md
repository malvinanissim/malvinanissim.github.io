---
layout: archive
permalink: /publications/
---

# Publications

My publications are listed below. You can also download a [full pdf](/assets/publications.pdf).

{% bibliography --style apa-no-doi-no-issue --file references  --reverse %}

<script>
function toggleBibtex(parameter) {
    var x= document.getElementById('a' + parameter);
    if (x.style.display === 'none') {
        x.style.display = 'block';
    } else {
        x.style.display = 'none';
    }
}
function toggleAbstract(parameter) {
    var x= document.getElementById('b' + parameter);
    if (x.style.display === 'none') {
        x.style.display = 'block';
    } else {
        x.style.display = 'none';
    }
}
</script>