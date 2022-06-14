---
theme: ./theme
class: text-center
highlighter: prism
info: |
  ## Slides for presenting online
drawings:
  persist: false
download: true
layout: intro
title: Test slides
themeConfig:
  # logoHeader: https://pic.imgdb.cn/item/62a835330947543129309526.png
  author: hehy
  authorUrl: https://www.lamda.nju.edu.cn/hehy
---

# Test Slidev


<div>
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Let's start <carbon:arrow-right class="inline"/>
  </span>
</div>


---
layout: presenter
presenterImage: >-
  https://avatars.githubusercontent.com/u/35964274?s=400&u=834d8e1f47668231cad95b4a2e2aa33008ade2e5&v=4
---

# Presenter: 
## A Handsome Man

<!--
这里少说话
-->

---
layout: text-window
reverse: true
---

# Embedded stuff

Use window to show a live demo of any page, or even a sub component!

::window::

<div class="overflow-hidden relative w-full aspect-16-9">
<iframe height="400" style="width: 100%;" scrolling="yes" title="Text Clock" src="https://www.bing.com" frameborder="yes" loading="lazy" allowtransparency="true" allowfullscreen="no" >
</iframe>
</div>

---

# Gracias totales

[Documentations](https://sli.dev) / [GitHub Repo](https://github.com/slidevjs/slidev)
