---
layout: page
permalink: /publications/index.html
title: Publications
pubs:
  - author: "Linhu Li, Eduardo V. Castro, Pedro D. Sacramento"
    title: "Strain induced topological phase transition at zigzag edges of monolayer transition-metal dichalcogenides"
    booktitle: "Phys. Rev. B (accepted)"
    url: https://arxiv.org/abs/1607.04337

  - author: "Linhu Li, Miguel A. N. Araújo"
    title: "Topological insulating phases from two-dimensional nodal loop semimetals"
    booktitle: "Phys. Rev. B 94, 165117 (2016)"
    url: https://journals.aps.org/prb/abstract/10.1103/PhysRevB.94.165117

  - author: "Linhu Li, Chao Yang, Shu Chen"
    title: "Topological invariants for phase transition points of one-dimensional Z2 topological systems"
    booktitle: "Eur. Phys. J. B (2016) 89: 195"
    url: http://link.springer.com/article/10.1140%2Fepjb%2Fe2016-70325-x

  - author: "Linhu Li, Chao Yang, Shu Chen"
    title: "Winding numbers of phase transition points for one-dimensional topological systems"
    booktitle: "EPL, 112 (2015) 10004"
    url: http://iopscience.iop.org/article/10.1209/0295-5075/112/10004/meta

  - author: "Linhu Li, Shu Chen"
    title: "Characterization of topological phase transitions via topological properties of transition points"
    url: "http://journals.aps.org/prb/abstract/10.1103/PhysRevB.92.085118"
    booktitle: "Phys. Rev. B 92, 085118 (2015)"

  - author: "Linhu Li, Shu Chen"
    title: "Hidden-symmetry-protected topological phases on a one-dimensional lattice"
    url: "http://iopscience.iop.org/article/10.1209/0295-5075/109/40006"
    booktitle: "EPL, 109 (2015) 40006"

  - author: "Linhu Li, Zhihao Xu, Shu Chen"
    title: "Topological phases of generalized Su-Schrieffer-Heeger models"
    url: "http://journals.aps.org/prb/abstract/10.1103/PhysRevB.89.085111"
    booktitle: "Phys. Rev. B 89, 085111 (2014)"

  - author: "Zhihao Xu, Linhu Li, Shu Chen"
    title: "Fractional topological states of dipolar fermions in one-dimensional optical superlattices"
    url: "http://journals.aps.org/prl/abstract/10.1103/PhysRevLett.110.215301"
    booktitle: "Phys. Rev. Lett. 110, 215301 (2013)"

  - author: "Zhihao Xu, Linhu Li, Gao Xianlong, Shu Chen"
    title: "Characterization of topological phase transitions via topological properties of transition points"
    url: "http://iopscience.iop.org/article/10.1088/0953-8984/25/5/055601/meta"
    booktitle: " J. Phys.: Condens. Matter 25 (2013) 055601"


---

# Publications

{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).
    {% else %} {{pub.title}}.
    {% endif %}{% if pub.type %}({{pub.type}})
    {% endif %}<br>
    {{pub.author}},
    {% if pub.type == 'Technical Report' %}{{pub.number}}
    {% endif %}{{pub.booktitle}}{{pub.school}}{{pub.journal}}.<br>
    {% if pub.address %}{{pub.address}}.
    {% endif %}{% if pub.key %}[Bibtex](http://groups.csail.mit.edu/commit/bibtex.cgi?key={{pub.key}}).
    {% endif %}{% if pub.bibtex %}[Bibtex]({{pub.bibtex}}).
    {% endif %}
{% endunless %}
{% endfor %}



