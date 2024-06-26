---
layout: archive
permalink: /publications/
---

# Publications

My publications are listed below. You can also download a [full pdf](/assets/publications.pdf).

<!-- 
to re-create updated pdf do this:
in Dropbox/Bureau/Biblio run:  sh makerefs.sh
A pdf will be generated from the "\_bibliography/references.bib" file and will be copied over 
to assets. Will need to be committed at next commit/push
-->


{% bibliography --file references  --reverse %}

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