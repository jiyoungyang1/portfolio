---
layout: sidebar
title: Publications
permalink: /publications/
---

<style>
.bibliography {
  list-style: none;
  padding: 0;
}

.bibliography li {
  position: relative;
  margin-bottom: 2em;
  padding-right: 180px;
  min-height: 150px;
}

.bibliography .preview {
  position: absolute;
  right: 0;
  top: 0;
  width: 160px;
  height: auto;
}

.bibliography .preview img {
  width: 100%;
  height: auto;
  border-radius: 4px;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

.bibliography .title {
  font-weight: bold;
  margin-bottom: 0.5em;
}

.bibliography .author {
  font-style: italic;
  margin-bottom: 0.5em;
}

.bibliography .periodical {
  margin-bottom: 0.5em;
}

.bibliography .links a {
  margin-right: 1em;
  color: #0366d6;
  text-decoration: none;
}

.bibliography .links a:hover {
  text-decoration: underline;
}

@media (max-width: 768px) {
  .bibliography li {
    padding-right: 0;
    min-height: auto;
  }

  .bibliography .preview {
    position: static;
    width: 100%;
    margin-top: 1em;
  }
}
</style>

{% bibliography %}
