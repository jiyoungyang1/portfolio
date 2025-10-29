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
  margin-bottom: 2.5em;
  padding-bottom: 2em;
  border-bottom: 1px solid #e1e4e8;
}

.bibliography li:last-child {
  border-bottom: none;
}

.bibliography-entry {
  position: relative;
  padding-right: 200px;
  min-height: 160px;
}

.bibliography-entry .preview {
  position: absolute;
  right: 0;
  top: 0;
  width: 180px;
  height: auto;
}

.bibliography-entry .preview img {
  width: 100%;
  height: auto;
  border-radius: 6px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.12);
  border: 1px solid #e1e4e8;
}

.bibliography-entry .bib-content {
  padding-right: 1em;
}

.bibliography-entry .badge {
  display: inline-block;
  background-color: #0366d6;
  color: white;
  padding: 0.2em 0.6em;
  border-radius: 3px;
  font-size: 0.75em;
  font-weight: bold;
  margin-bottom: 0.5em;
  margin-right: 0.5em;
}

.bibliography-entry .title {
  font-weight: 600;
  font-size: 1.1em;
  color: #24292e;
  margin-bottom: 0.5em;
  line-height: 1.4;
}

.bibliography-entry .author {
  color: #586069;
  margin-bottom: 0.5em;
  font-size: 0.95em;
}

.bibliography-entry .periodical {
  color: #24292e;
  margin-bottom: 0.75em;
  font-size: 0.9em;
}

.bibliography-entry .periodical em {
  font-style: italic;
}

.bibliography-entry .abstract {
  margin: 0.75em 0;
}

.bibliography-entry .abstract details {
  background-color: #f6f8fa;
  padding: 0.5em 0.75em;
  border-radius: 4px;
  border: 1px solid #e1e4e8;
}

.bibliography-entry .abstract summary {
  cursor: pointer;
  font-weight: 500;
  color: #0366d6;
  font-size: 0.9em;
}

.bibliography-entry .abstract summary:hover {
  text-decoration: underline;
}

.bibliography-entry .abstract p {
  margin-top: 0.75em;
  color: #24292e;
  font-size: 0.9em;
  line-height: 1.6;
}

.bibliography-entry .links {
  margin-top: 0.75em;
}

.bibliography-entry .links a {
  display: inline-block;
  margin-right: 1em;
  color: #0366d6;
  text-decoration: none;
  font-size: 0.9em;
  font-weight: 500;
}

.bibliography-entry .links a:hover {
  text-decoration: underline;
}

.bibliography-entry .note {
  margin-top: 0.5em;
  color: #6a737d;
  font-size: 0.85em;
}

@media (max-width: 768px) {
  .bibliography-entry {
    padding-right: 0;
    min-height: auto;
  }

  .bibliography-entry .preview {
    position: static;
    width: 100%;
    max-width: 300px;
    margin: 1em auto;
    display: block;
  }

  .bibliography-entry .bib-content {
    padding-right: 0;
  }
}
</style>

{% bibliography %}
