---
layout: archive
permalink: /publications/
---

# Publications
My publications are listed below. You can also download a [full pdf](/assets/publications.pdf) (most recent first).

{% bibliography --query @*[year<=2024]--style apa --file references  --reverse %}

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