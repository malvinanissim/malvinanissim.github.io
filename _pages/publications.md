---
layout: archive
permalink: /publications/
---

# Publications
You can also download a [full pdf](/assets/publications.pdf) (most recent first).


{% bibliography --style apa --file references %}

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